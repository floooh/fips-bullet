# fips-bullet

fips wrapper for Bullet physics (https://github.com/bulletphysics/bullet3.git)

fips build system: https://github.com/floooh/fips

This wrapper only exposes the Bullet2 APIs (Collision, Dynamics, SoftBody, LinearMath)!

### How to integrate into your fips project:

Add the following import to your fips.yml:

```yaml
imports:
    fips-bullet:
        git: https://github.com/floooh/fips-bullet.git
```

Add the dependency _Bullet_ to your app's CMakeLists.txt file:

```cmake
fips_begin_app(MyApp windowed)
    ...
    fips_deps(Bullet)
    ...
fips_end_app()
```

