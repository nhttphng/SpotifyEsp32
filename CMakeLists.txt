idf_component_register(
  SRCS "src/SpotifyEsp32.cpp"
  INCLUDE_DIRS "src"
  REQUIRES arduino-esp32 ArduinoJson
)

target_compile_options(${COMPONENT_LIB} PRIVATE
  -Wno-error=address
  -Wno-error=format-truncation
)