# Retainer

The retainer is intended to optimize what is painted to the screen.
Since the rasterizer may be out-of-sync with the screen, this layer uses double-buffering to achieve smooth repainting.
Especially in 2d graphics, only small regions of the screen actually change.
In 3d, this layer can also be responsible for occlusion culling to avoid painting hidden objects.
[Painter's algorithm](https://en.wikipedia.org/wiki/Painter%27s_algorithm) is often used to prevent overpainting. 
