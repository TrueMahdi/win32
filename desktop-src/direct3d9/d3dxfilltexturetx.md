---
Description: Uses a compiled high-level shader language (HLSL) function to fill each texel of each mipmap level of a texture.
ms.assetid: 013660ce-865e-4acf-a1ea-670e70377ff5
title: D3DXFillTextureTX function
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# D3DXFillTextureTX function

Uses a compiled high-level shader language (HLSL) function to fill each texel of each mipmap level of a texture.

## Syntax


```C++
HRESULT D3DXFillTextureTX(
  _Inout_ LPDIRECT3DTEXTURE9  pTexture,
  _In_    LPD3DXTEXTURESHADER pTextureShader
);
```



## Parameters

<dl> <dt>

*pTexture* \[in, out\]
</dt> <dd>

Type: **[**LPDIRECT3DTEXTURE9**](/windows/desktop/api/d3d9helper/nn-d3d9-idirect3dtexture9)**

Pointer to an [**IDirect3DTexture9**](/windows/desktop/api/d3d9helper/nn-d3d9-idirect3dtexture9) object, representing the texture to be filled.

</dd> <dt>

*pTextureShader* \[in\]
</dt> <dd>

Type: **[**LPD3DXTEXTURESHADER**](id3dxtextureshader.md)**

Pointer to a [**ID3DXTextureShader**](id3dxtextureshader.md) texture shader object.

</dd> </dl>

## Return value

Type: **[**HRESULT**](https://msdn.microsoft.com/windows/desktop/455d07e9-52c3-4efb-a9dc-2955cbfd38cc)**

If the function succeeds, the return value is D3D\_OK. If the function fails, the return value can be one of the following: D3DERR\_NOTAVAILABLE, D3DERR\_INVALIDCALL.

## Remarks

The texture target must be an HLSL function that takes contains the following semantics:

-   One input parameter must use a POSITION semantic.
-   One input parameter must use a PSIZE semantic.
-   The function must return a parameter that uses the COLOR semantic.

The following is an example of such an HLSL function:


```
float4 TextureGradientFill(
  float2 vTexCoord : POSITION, 
  float2 vTexelSize : PSIZE) : COLOR 
  {
    float r,g, b, xSq,ySq, a;
    xSq = 2.f*vTexCoord.x-1.f; xSq *= xSq;
    ySq = 2.f*vTexCoord.y-1.f; ySq *= ySq;
    a = sqrt(xSq+ySq);
    if (a > 1.0f) {
        a = 1.0f-(a-1.0f);
    }
    else if (a < 0.2f) {
        a = 0.2f;
    }
    r = 1-vTexCoord.x;
    g = 1-vTexCoord.y;
    b = vTexCoord.x;
    return float4(r, g, b, a);
    
  };
```



Note that the input parameters can be in any order, but both input semantics must be represented.

## Requirements



|                    |                                                                                       |
|--------------------|---------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>D3dx9tex.h</dt> </dl> |
| Library<br/> | <dl> <dt>D3dx9.lib</dt> </dl>  |



## See also

<dl> <dt>

[Texture Functions in D3DX 9](dx9-graphics-reference-d3dx-functions-texture.md)
</dt> <dt>

[**D3DXFillCubeTextureTX**](d3dxfillcubetexturetx.md)
</dt> <dt>

[**D3DXFillVolumeTextureTX**](d3dxfillvolumetexturetx.md)
</dt> </dl>

 

 



