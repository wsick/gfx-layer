# Rasterizer

The rasterization layer is necessary to flatten vector graphics into a flat image for on-screen display.
Even when images have already been rasterized, graphics systems typically composite multiple rasterizations.

This layer is an immediate mode (paint directly to a buffer) phase that grants any GUI the ability to be resolution independent and hardware accelerated.
Rasterizers (2d) commonly achieve hardware acceleration by projecting flat textures in a 3d space using an orthogonal camera.
This contrasts with software-accelerated systems that are using algorithms to convert shape primitives into pixels.
This also has the advantage of using the camera transforms to "zoom in" and "zoom out" of a scene.
