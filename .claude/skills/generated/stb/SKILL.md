---
name: stb
description: "Skill for the Stb area of cmux-gtk. 233 symbols across 2 files."
---

# Stb

233 symbols | 2 files | Cohesion: 68%

## When to Use

- Working with code in `ghostty/`
- Understanding how stbir_resize_uint8, stbir_resize_float, stbir_resize_uint8_srgb work
- Modifying stb-related functionality

## Key Files

| File | Symbols |
|------|---------|
| `ghostty/src/stb/stb_image.h` | stbi__bitreverse16, stbi__bit_reverse, stbi__zbuild_huffman, stbi__zeof, stbi__zget8 (+174) |
| `ghostty/src/stb/stb_image_resize.h` | stbir_resize_uint8, stbir_resize_float, stbir_resize_uint8_srgb, stbir_resize_uint8_srgb_edgemode, stbir_resize_uint8_generic (+49) |

## Entry Points

Start here when exploring this area:

- **`stbir_resize_uint8`** (Function) — `ghostty/src/stb/stb_image_resize.h:227`
- **`stbir_resize_float`** (Function) — `ghostty/src/stb/stb_image_resize.h:231`
- **`stbir_resize_uint8_srgb`** (Function) — `ghostty/src/stb/stb_image_resize.h:252`
- **`stbir_resize_uint8_srgb_edgemode`** (Function) — `ghostty/src/stb/stb_image_resize.h:266`
- **`stbir_resize_uint8_generic`** (Function) — `ghostty/src/stb/stb_image_resize.h:306`

## Key Symbols

| Symbol | Type | File | Line |
|--------|------|------|------|
| `stbir_resize_uint8` | Function | `ghostty/src/stb/stb_image_resize.h` | 227 |
| `stbir_resize_float` | Function | `ghostty/src/stb/stb_image_resize.h` | 231 |
| `stbir_resize_uint8_srgb` | Function | `ghostty/src/stb/stb_image_resize.h` | 252 |
| `stbir_resize_uint8_srgb_edgemode` | Function | `ghostty/src/stb/stb_image_resize.h` | 266 |
| `stbir_resize_uint8_generic` | Function | `ghostty/src/stb/stb_image_resize.h` | 306 |
| `stbir_resize_uint16_generic` | Function | `ghostty/src/stb/stb_image_resize.h` | 312 |
| `stbir_resize_float_generic` | Function | `ghostty/src/stb/stb_image_resize.h` | 318 |
| `stbir_resize` | Function | `ghostty/src/stb/stb_image_resize.h` | 349 |
| `stbir_resize_subpixel` | Function | `ghostty/src/stb/stb_image_resize.h` | 357 |
| `stbir_resize_region` | Function | `ghostty/src/stb/stb_image_resize.h` | 367 |
| `stbi_zlib_decode_malloc_guesssize` | Function | `ghostty/src/stb/stb_image.h` | 526 |
| `stbi_zlib_decode_malloc_guesssize_headerflag` | Function | `ghostty/src/stb/stb_image.h` | 527 |
| `stbi_zlib_decode_buffer` | Function | `ghostty/src/stb/stb_image.h` | 529 |
| `stbi_zlib_decode_noheader_malloc` | Function | `ghostty/src/stb/stb_image.h` | 531 |
| `stbi_zlib_decode_noheader_buffer` | Function | `ghostty/src/stb/stb_image.h` | 532 |
| `stbi_loadf_from_memory` | Function | `ghostty/src/stb/stb_image.h` | 455 |
| `stbi_is_hdr_from_memory` | Function | `ghostty/src/stb/stb_image.h` | 476 |
| `stbi_is_16_bit_from_memory` | Function | `ghostty/src/stb/stb_image.h` | 493 |
| `stbi_is_16_bit_from_callbacks` | Function | `ghostty/src/stb/stb_image.h` | 494 |
| `stbi_is_16_bit_from_file` | Function | `ghostty/src/stb/stb_image.h` | 500 |

## Execution Flows

| Flow | Type | Steps |
|------|------|-------|
| `Stbi__bmp_load → Stbi__get8` | cross_community | 5 |
| `Stbi__psd_load → Stbi__get8` | cross_community | 4 |
| `Stbi__hdr_load → Stbi__mul2sizes_valid` | intra_community | 4 |
| `Stbi__hdr_load → Stbi__addsizes_valid` | intra_community | 4 |
| `Stbi__hdr_load → STBI_MALLOC` | cross_community | 4 |

## How to Explore

1. `gitnexus_context({name: "stbir_resize_uint8"})` — see callers and callees
2. `gitnexus_query({query: "stb"})` — find related execution flows
3. Read key files listed above for implementation details
