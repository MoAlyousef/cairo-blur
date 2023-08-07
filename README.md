# cairo-blur

Apply a Gaussian blur to your Cairo ImageSurface.

```rust,ignore
let radius = 15;
let mut surf = cairo::ImageSurface::create(Format::ARgb32, 200, 100).expect("Couldn’t create surface");
cairo_blur::blur_image_surface(&mut surf, radius);
```