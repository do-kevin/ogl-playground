# Performance notes

Tips for optimization when it comes to WebGL.

If your application is freezing a bit, especially during page transitions, it means the textures are being loaded into the GPU.

So we want to use a throbber and preload all the images and shaders before the page is shown. It should be a smoother experience and reduces flickering.

And then remember to destroy previous scenes when you transition to a different page.
