# exampletiffs

These are some examples that showcase features of the TIFF format in order
to thoroughly test TIFF.jl.

Unfortunately the copyright information for several of these tifs is
unknown.

| Name                                   | Source            | Size (Rows, Cols)   | Features                                | License                                                         |
|----------------------------------------|-------------------|---------------------|-----------------------------------------|-----------------------------------------------------------------|        
| `bali.tif`                             | [1]               | (489, 725)          | LZW compression, RGB                    | ?                                                               |
| `underwater_bmx.tif`                   | [1]               | (1076, 773)         | Adobe Deflate compression, RGB          | ?                                                               |
| `spine.tif`                            | [1]               | (637, 490)          | Packbits compression, RGB               | ?                                                               |
| `flagler.tif`                          | [1]               | (200, 541)          | RGBA                                    | ?                                                               |
| `mri.tif`                              | [1]               | (128, 128, 27)      | 3 dimensions, Packbits compression, RGB | ?                                                               |
| `spring.tif`                           | Tamas Nagy        | (619, 858)          | Float16 RGB                             | [BSD-3-Clause](https://opensource.org/licenses/BSD-3-Clause)    |
| `poppies.tif`                          | Tamas Nagy        | (1008, 756)         | Rotated orientation, Palette-colored    | [BSD-3-Clause](https://opensource.org/licenses/BSD-3-Clause)    |
| `capitol.tif`                          | Tamas Nagy        | (378, 504)          | Bilevel image                           | [BSD-3-Clause](https://opensource.org/licenses/BSD-3-Clause)    |
| `capitol2.tif`                         | Tamas Nagy        | (378, 504)          | Striped bilevel image                   | [BSD-3-Clause](https://opensource.org/licenses/BSD-3-Clause)    |
| `coffee.tif`                           | Tamas Nagy        | (378, 504)          | Grayscale, Packbits                     | [BSD-3-Clause](https://opensource.org/licenses/BSD-3-Clause)    |
| `house.tif`                            | [2]               | (512, 512)          | Gray Alpha                              | MIT license?                                                    |
| `4D-series.ome.tif`                    | [3]               | (439, 167, 5, 1, 7) | Signed integer gray type                | [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)       |
| `julia.tif`                            | Tamas Nagy        | (378, 504)          | RGB, discontiguous strips [4]           | [BSD-3-Clause](https://opensource.org/licenses/BSD-3-Clause)    |
| `shapes_uncompressed.tif`              | Christopher Burns | (128, 72)           | uncompressed [5]                        | [BSD-3-Clause](https://opensource.org/licenses/BSD-3-Clause)    |
| `shapes_deflate.tif`                   | Christopher Burns | (128, 72)           | Adobe Deflate Compression [5]           | [BSD-3-Clause](https://opensource.org/licenses/BSD-3-Clause)    |
| `shapes_lzw.tif`                       | Christopher Burns | (128, 72)           | LZW Compression [5]                     | [BSD-3-Clause](https://opensource.org/licenses/BSD-3-Clause)    |
| `shapes_lzw_tiled.tif`                 | Christopher Burns | (128, 72)           | Tiled, LZW Compression [5]              | [BSD-3-Clause](https://opensource.org/licenses/BSD-3-Clause)    |
| `shapes_lzw_planar.tif`                | Christopher Burns | (128, 72)           | Planar, LZW Compression [5]             | [BSD-3-Clause](https://opensource.org/licenses/BSD-3-Clause)    |
| `shapes_lzw_tiled_planar.tif`          | Christopher Burns | (128, 72)           | Tiled, Planar, LZW Compression [5]      | [BSD-3-Clause](https://opensource.org/licenses/BSD-3-Clause)    |
| `shapes_umcompressed_tiled_planar.tif` | Christopher Burns | (128, 72)           | Tiled, Planar, Uncompressed [5]         | [BSD-3-Clause](https://opensource.org/licenses/BSD-3-Clause)    |
| `shapes_lzw_12bps.tif`                 | Christopher Burns | (128, 72)           | LZW, 12 bits per channel [5]            | [BSD-3-Clause](https://opensource.org/licenses/BSD-3-Clause)    |
| `shapes_lzw_planar_10bps.tif`          | Christopher Burns | (128, 72)           | Planar, LZW, 10 bits per channel [5]    | [BSD-3-Clause](https://opensource.org/licenses/BSD-3-Clause)    |
| `shapes_lzw_14bps.tif`                 | Christopher Burns | (128, 72)           | LZW, 14 bits per channel [5]            | [BSD-3-Clause](https://opensource.org/licenses/BSD-3-Clause)    |
| `shapes_lzw_predictor3.tif`            | Christopher Burns | (128, 72)           | predictor == 3, LZW Compression [5]     | [BSD-3-Clause](https://opensource.org/licenses/BSD-3-Clause)    |
| `earthlab.tif`                         | Earth Lab         | (2400, 2400)        | LZW, codesize change on boundary [6]    | [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) |

[1]: http://people.math.sc.edu/Burkardt/data/tif/tif.html
[2]: https://github.com/JuliaImages/TestImages.jl
[3]: https://docs.openmicroscopy.org/ome-model/6.0.0/ome-tiff/data.html
[4]: https://github.com/tlnagy/TiffImages.jl/pull/38#issuecomment-786281834
[5]: all shapes_* images are identical and differ only by encoding
[6]: https://www.earthdatascience.org/courses/use-data-open-source-python/multispectral-remote-sensing/landsat-in-Python/
