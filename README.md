This is a small project to show and reproduce a problem that occurs when compiling the boilerplate code generated by 
the `esp-rs/esp-idf-template`

To reproduce:


`cargo generate esp-rs/esp-idf-template cargo`

project name `prob-idf`, MCU target `esp32c3` esp_idf_version = 5.2.2 and otherwise default options:

![options](cargo-esp-generate.png)

```
cd prob-idf
cargo build |& tee cargo_build.log
```

The build logs and resulting error is visible in [cargo_build.log](cargo_build.log)


