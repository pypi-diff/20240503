# Comparing `tmp/slint-1.6.0a6.tar.gz` & `tmp/slint-1.6.0a7.tar.gz`

## Comparing `slint-1.6.0a6.tar` & `slint-1.6.0a7.tar`

### file list

```diff
@@ -1,888 +1,894 @@
--rw-r--r--   0     1001      127     3852 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/winit/Cargo.toml
--rw-r--r--   0     1001      127    34670 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/winit/LICENSES/GPL-3.0-only.txt
--rw-r--r--   0     1001      127     3475 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/winit/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
--rw-r--r--   0     1001      127    14063 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/winit/LICENSES/LicenseRef-Slint-commercial.md
--rw-r--r--   0     1001      127     2320 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/winit/README.md
--rw-r--r--   0     1001      127    21942 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/winit/accesskit.rs
--rw-r--r--   0     1001      127      474 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/winit/build.rs
--rw-r--r--   0     1001      127    30209 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/winit/event_loop.rs
--rw-r--r--   0     1001      127    16654 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/winit/lib.rs
--rw-r--r--   0     1001      127     8046 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/winit/renderer/femtovg/glcontext.rs
--rw-r--r--   0     1001      127     2131 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/winit/renderer/femtovg.rs
--rw-r--r--   0     1001      127     4558 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/winit/renderer/skia.rs
--rw-r--r--   0     1001      127     6824 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/winit/renderer/sw.rs
--rw-r--r--   0     1001      127    14717 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/winit/wasm_input_helper.rs
--rw-r--r--   0     1001      127    32085 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/winit/winitwindowadapter.rs
--rw-r--r--   0     1001      127     4483 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/Cargo.toml
--rw-r--r--   0     1001      127    34670 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/LICENSES/GPL-3.0-only.txt
--rw-r--r--   0     1001      127     3475 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
--rw-r--r--   0     1001      127    14063 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/LICENSES/LicenseRef-Slint-commercial.md
--rw-r--r--   0     1001      127      532 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/README.md
--rw-r--r--   0     1001      127     2766 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/accessibility.rs
--rw-r--r--   0     1001      127    13996 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/animations.rs
--rw-r--r--   0     1001      127    38608 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/api.rs
--rw-r--r--   0     1001      127     5210 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/callbacks.rs
--rw-r--r--   0     1001      127     2586 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/component_factory.rs
--rw-r--r--   0     1001      127     2553 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/context.rs
--rw-r--r--   0     1001      127     7694 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/future.rs
--rw-r--r--   0     1001      127     2503 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/graphics/bitmapfont.rs
--rw-r--r--   0     1001      127    14664 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/graphics/border_radius.rs
--rw-r--r--   0     1001      127     4038 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/graphics/boxshadowcache.rs
--rw-r--r--   0     1001      127    14919 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/graphics/brush.rs
--rw-r--r--   0     1001      127    17436 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/graphics/color.rs
--rw-r--r--   0     1001      127     7064 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/graphics/image/cache.rs
--rw-r--r--   0     1001      127     2528 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/graphics/image/htmlimage.rs
--rw-r--r--   0     1001      127     3408 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/graphics/image/svg.rs
--rw-r--r--   0     1001      127    48855 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/graphics/image.rs
--rw-r--r--   0     1001      127    15911 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/graphics/path.rs
--rw-r--r--   0     1001      127     6978 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/graphics/rendering_metrics_collector.rs
--rw-r--r--   0     1001      127     8021 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/graphics.rs
--rw-r--r--   0     1001      127    33891 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/input.rs
--rw-r--r--   0     1001      127     8604 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/item_focus.rs
--rw-r--r--   0     1001      127    29328 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/item_rendering.rs
--rw-r--r--   0     1001      127    67985 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/item_tree.rs
--rw-r--r--   0     1001      127     8608 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/items/component_container.rs
--rw-r--r--   0     1001      127    17039 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/items/flickable.rs
--rw-r--r--   0     1001      127     8722 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/items/image.rs
--rw-r--r--   0     1001      127     5377 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/items/path.rs
--rw-r--r--   0     1001      127    65770 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/items/text.rs
--rw-r--r--   0     1001      127    46631 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/items.rs
--rw-r--r--   0     1001      127    27945 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/layout.rs
--rw-r--r--   0     1001      127     3222 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/lengths.rs
--rw-r--r--   0     1001      127     2237 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/lib.rs
--rw-r--r--   0     1001      127    47643 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/model/adapters.rs
--rw-r--r--   0     1001      127     6658 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/model/model_peer.rs
--rw-r--r--   0     1001      127    47290 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/model.rs
--rw-r--r--   0     1001      127    15948 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/platform.rs
--rw-r--r--   0     1001      127    15736 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/properties/ffi.rs
--rw-r--r--   0     1001      127    38401 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/properties/properties_animations.rs
--rw-r--r--   0     1001      127    58572 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/properties.rs
--rw-r--r--   0     1001      127     5015 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/renderer.rs
--rw-r--r--   0     1001      127    10886 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/rtti.rs
--rw-r--r--   0     1001      127    21418 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/sharedvector.rs
--rw-r--r--   0     1001      127     2865 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/slice.rs
--rw-r--r--   0     1001      127    29158 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/software_renderer/draw_functions.rs
--rw-r--r--   0     1001      127     3465 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/software_renderer/fixed.rs
--rw-r--r--   0     1001      127     4673 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/software_renderer/fonts/pixelfont.rs
--rw-r--r--   0     1001      127     3859 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/software_renderer/fonts/systemfonts.rs
--rw-r--r--   0     1001      127     7334 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/software_renderer/fonts/vectorfont.rs
--rw-r--r--   0     1001      127     5915 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/software_renderer/fonts.rs
--rw-r--r--   0     1001      127    99070 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/software_renderer.rs
--rw-r--r--   0     1001      127    13307 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/string.rs
--rw-r--r--   0     1001      127     4121 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/tests.rs
--rw-r--r--   0     1001      127    12929 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/textlayout/fragments.rs
--rw-r--r--   0     1001      127     3222 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/textlayout/glyphclusters.rs
--rw-r--r--   0     1001      127     1234 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/textlayout/linebreak_simple.rs
--rw-r--r--   0     1001      127     1260 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/textlayout/linebreak_unicode.rs
--rw-r--r--   0     1001      127    15364 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/textlayout/linebreaker.rs
--rw-r--r--   0     1001      127    13512 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/textlayout/shaping.rs
--rw-r--r--   0     1001      127    24952 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/textlayout.rs
--rw-r--r--   0     1001      127    31468 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/timers.rs
--rw-r--r--   0     1001      127     8559 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/translations.rs
--rw-r--r--   0     1001      127     1884 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/unsafe_single_threaded.rs
--rw-r--r--   0     1001      127    62402 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core/window.rs
--rw-r--r--   0     1001      127     1913 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/Cargo.toml
--rw-r--r--   0     1001      127    10280 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/LICENSES/Apache-2.0.txt
--rw-r--r--   0     1001      127    16830 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/LICENSES/CC-BY-ND-4.0.txt
--rw-r--r--   0     1001      127    34670 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/LICENSES/GPL-3.0-only.txt
--rw-r--r--   0     1001      127     3475 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
--rw-r--r--   0     1001      127    14063 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/LICENSES/LicenseRef-Slint-commercial.md
--rw-r--r--   0     1001      127     1078 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/LICENSES/MIT.txt
--rw-r--r--   0     1001      127      537 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/README.md
--rw-r--r--   0     1001      127     2420 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/build.rs
--rw-r--r--   0     1001      127    16358 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/builtin_macros.rs
--rw-r--r--   0     1001      127    18381 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/builtins.slint
--rw-r--r--   0     1001      127    19587 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/diagnostics.rs
--rw-r--r--   0     1001      127     2636 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/embedded_resources.rs
--rw-r--r--   0     1001      127    69622 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/expression_tree.rs
--rw-r--r--   0     1001      127     4420 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/fileaccess.rs
--rw-r--r--   0     1001      127   139818 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/generator/cpp.rs
--rw-r--r--   0     1001      127   122025 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/generator/rust.rs
--rw-r--r--   0     1001      127    19509 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/generator.rs
--rw-r--r--   0     1001      127    32752 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/langtype.rs
--rw-r--r--   0     1001      127    21425 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/layout.rs
--rw-r--r--   0     1001      127    15374 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/lexer.rs
--rw-r--r--   0     1001      127     9399 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/lib.rs
--rw-r--r--   0     1001      127     7020 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/literals.rs
--rw-r--r--   0     1001      127    31386 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/llr/expression.rs
--rw-r--r--   0     1001      127    13363 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/llr/item_tree.rs
--rw-r--r--   0     1001      127    40541 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/llr/lower_expression.rs
--rw-r--r--   0     1001      127    31339 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/llr/lower_to_item_tree.rs
--rw-r--r--   0     1001      127     6314 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/llr/optim_passes/count_property_use.rs
--rw-r--r--   0     1001      127     6235 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/llr/optim_passes/inline_expressions.rs
--rw-r--r--   0     1001      127    11380 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/llr/pretty_print.rs
--rw-r--r--   0     1001      127      654 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/llr.rs
--rw-r--r--   0     1001      127    11758 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/load_builtins.rs
--rw-r--r--   0     1001      127    39783 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/lookup.rs
--rw-r--r--   0     1001      127     7518 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/namedreference.rs
--rw-r--r--   0     1001      127   101372 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/object_tree.rs
--rw-r--r--   0     1001      127    10913 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/parser/document.rs
--rw-r--r--   0     1001      127    20594 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/parser/element.rs
--rw-r--r--   0     1001      127    14696 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/parser/expressions.rs
--rw-r--r--   0     1001      127     3102 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/parser/statements.rs
--rw-r--r--   0     1001      127     4561 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/parser/type.rs
--rw-r--r--   0     1001      127    36188 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/parser.rs
--rw-r--r--   0     1001      127     3949 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/apply_default_properties_from_style.rs
--rw-r--r--   0     1001      127    22379 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/binding_analysis.rs
--rw-r--r--   0     1001      127     1587 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/border_radius.rs
--rw-r--r--   0     1001      127     1793 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/check_expressions.rs
--rw-r--r--   0     1001      127     1941 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/check_public_api.rs
--rw-r--r--   0     1001      127     2309 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/check_rotation.rs
--rw-r--r--   0     1001      127     4580 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/clip.rs
--rw-r--r--   0     1001      127     2464 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/collect_custom_fonts.rs
--rw-r--r--   0     1001      127     1933 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/collect_globals.rs
--rw-r--r--   0     1001      127     1150 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/collect_init_code.rs
--rw-r--r--   0     1001      127     4172 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/collect_structs_and_enums.rs
--rw-r--r--   0     1001      127     1392 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/collect_subcomponents.rs
--rw-r--r--   0     1001      127     8043 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/compile_paths.rs
--rw-r--r--   0     1001      127     9466 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/const_propagation.rs
--rw-r--r--   0     1001      127     6155 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/deduplicate_property_read.rs
--rw-r--r--   0     1001      127    18877 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/default_geometry.rs
--rw-r--r--   0     1001      127    16260 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/embed_glyphs.rs
--rw-r--r--   0     1001      127    14883 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/embed_images.rs
--rw-r--r--   0     1001      127     5111 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/ensure_window.rs
--rw-r--r--   0     1001      127     6270 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/flickable.rs
--rw-r--r--   0     1001      127    10032 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/focus_handling.rs
--rw-r--r--   0     1001      127     4318 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/generate_item_indices.rs
--rw-r--r--   0     1001      127     6709 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/infer_aliases_types.rs
--rw-r--r--   0     1001      127    21709 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/inlining.rs
--rw-r--r--   0     1001      127     3241 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/lower_absolute_coordinates.rs
--rw-r--r--   0     1001      127     3268 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/lower_accessibility.rs
--rw-r--r--   0     1001      127     1697 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/lower_component_container.rs
--rw-r--r--   0     1001      127    31672 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/lower_layout.rs
--rw-r--r--   0     1001      127     5565 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/lower_popups.rs
--rw-r--r--   0     1001      127     5182 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/lower_property_to_element.rs
--rw-r--r--   0     1001      127     6916 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/lower_shadows.rs
--rw-r--r--   0     1001      127     9988 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/lower_states.rs
--rw-r--r--   0     1001      127     8355 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/lower_tabwidget.rs
--rw-r--r--   0     1001      127     2000 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/lower_text_input_interface.rs
--rw-r--r--   0     1001      127     6185 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/materialize_fake_properties.rs
--rw-r--r--   0     1001      127     6748 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/move_declarations.rs
--rw-r--r--   0     1001      127     2749 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/optimize_useless_rectangles.rs
--rw-r--r--   0     1001      127     4231 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/purity_check.rs
--rw-r--r--   0     1001      127     9197 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/remove_aliases.rs
--rw-r--r--   0     1001      127    19427 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/remove_return.rs
--rw-r--r--   0     1001      127     1656 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/remove_unused_properties.rs
--rw-r--r--   0     1001      127     5067 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/repeater_component.rs
--rw-r--r--   0     1001      127     5620 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/resolve_native_classes.rs
--rw-r--r--   0     1001      127    70883 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/resolving.rs
--rw-r--r--   0     1001      127     3046 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/unique_id.rs
--rw-r--r--   0     1001      127     4210 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/visible.rs
--rw-r--r--   0     1001      127     2961 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes/z_order.rs
--rw-r--r--   0     1001      127    10533 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/passes.rs
--rw-r--r--   0     1001      127    18378 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/pathutils.rs
--rw-r--r--   0     1001      127     8412 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/consistent_styles.rs
--rw-r--r--   0     1001      127     1237 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/accessibility/accessible_properties.slint
--rw-r--r--   0     1001      127     1774 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/analysis/binding_loop1.slint
--rw-r--r--   0     1001      127     1826 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/analysis/binding_loop2.slint
--rw-r--r--   0     1001      127      924 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/analysis/binding_loop_function.slint
--rw-r--r--   0     1001      127      643 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/analysis/binding_loop_issue_772.slint
--rw-r--r--   0     1001      127     2458 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/analysis/binding_loop_layout.slint
--rw-r--r--   0     1001      127     1854 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/analysis/binding_loop_layout2.slint
--rw-r--r--   0     1001      127     1144 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/analysis/binding_loop_layout3.slint
--rw-r--r--   0     1001      127     2120 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/analysis/binding_loop_layout4.slint
--rw-r--r--   0     1001      127      488 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/analysis/binding_loop_mappointtowindow.slint
--rw-r--r--   0     1001      127      923 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/analysis/binding_loop_self.slint
--rw-r--r--   0     1001      127      942 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/animate.slint
--rw-r--r--   0     1001      127      230 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/array.slint
--rw-r--r--   0     1001      127      788 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/assign.slint
--rw-r--r--   0     1001      127      585 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/box_shadow.slint
--rw-r--r--   0     1001      127     1021 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/children_placeholder.slint
--rw-r--r--   0     1001      127      301 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/children_placeholder_2.slint
--rw-r--r--   0     1001      127      663 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/clip.slint
--rw-r--r--   0     1001      127      492 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/comments.slint
--rw-r--r--   0     1001      127     2078 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/dialog.slint
--rw-r--r--   0     1001      127      631 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/dialog2.slint
--rw-r--r--   0     1001      127      499 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/double_binding.slint
--rw-r--r--   0     1001      127      270 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/double_color.slint
--rw-r--r--   0     1001      127     1137 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/duplicated_id.slint
--rw-r--r--   0     1001      127     1340 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/easing.slint
--rw-r--r--   0     1001      127      383 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/easing_not_called.slint
--rw-r--r--   0     1001      127      156 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/empty.slint
--rw-r--r--   0     1001      127      526 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/enums.slint
--rw-r--r--   0     1001      127      441 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/for.slint
--rw-r--r--   0     1001      127      492 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/image.slint
--rw-r--r--   0     1001      127      450 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/inline_component.slint
--rw-r--r--   0     1001      127      895 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/item_as_property.slint
--rw-r--r--   0     1001      127      465 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/layout.slint
--rw-r--r--   0     1001      127     1958 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/layout2.slint
--rw-r--r--   0     1001      127     2188 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/linear-gradient.slint
--rw-r--r--   0     1001      127      470 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/object_in_binding.slint
--rw-r--r--   0     1001      127      538 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/opacity.slint
--rw-r--r--   0     1001      127      905 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/parse_error.slint
--rw-r--r--   0     1001      127      535 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/path.slint
--rw-r--r--   0     1001      127     1114 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/path_commands.slint
--rw-r--r--   0     1001      127      541 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/path_for.slint
--rw-r--r--   0     1001      127     1056 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/percent.slint
--rw-r--r--   0     1001      127      707 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/popup.slint
--rw-r--r--   0     1001      127      333 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/property_animation.slint
--rw-r--r--   0     1001      127      983 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/property_declaration.slint
--rw-r--r--   0     1001      127      268 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/property_declaration_in_component.slint
--rw-r--r--   0     1001      127     1786 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/radial-gradient.slint
--rw-r--r--   0     1001      127      837 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/return.slint
--rw-r--r--   0     1001      127     1850 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/rotation.slint
--rw-r--r--   0     1001      127      456 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/rust-attr.slint
--rw-r--r--   0     1001      127     1781 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/self_assign.slint
--rw-r--r--   0     1001      127     1413 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/signal.slint
--rw-r--r--   0     1001      127     4436 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/states_transitions.slint
--rw-r--r--   0     1001      127      711 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/states_transitions2.slint
--rw-r--r--   0     1001      127      748 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/states_transitions3.slint
--rw-r--r--   0     1001      127      731 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/states_two_way.slint
--rw-r--r--   0     1001      127      731 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/sub_elements.slint
--rw-r--r--   0     1001      127      218 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/supersimple.slint
--rw-r--r--   0     1001      127      467 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/svg_path.slint
--rw-r--r--   0     1001      127     1600 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/tr.slint
--rw-r--r--   0     1001      127     3038 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/tr2.slint
--rw-r--r--   0     1001      127     1108 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/type_declaration.slint
--rw-r--r--   0     1001      127     1391 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/basic/unknown_item.slint
--rw-r--r--   0     1001      127      457 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/callbacks/init.slint
--rw-r--r--   0     1001      127      671 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/elements/component_container.slint
--rw-r--r--   0     1001      127     1202 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/elements/listview.slint
--rw-r--r--   0     1001      127      601 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/elements/popup.slint
--rw-r--r--   0     1001      127      538 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/elements/tabwidget.slint
--rw-r--r--   0     1001      127      898 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/elements/tabwidget2.slint
--rw-r--r--   0     1001      127      474 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/elements/tabwidget3.slint
--rw-r--r--   0     1001      127      436 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/exports/export_duplicates.slint
--rw-r--r--   0     1001      127      623 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/exports/reexport_duplicate.slint
--rw-r--r--   0     1001      127      326 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/exports/root_compo_export.slint
--rw-r--r--   0     1001      127      289 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/exports/root_compo_export2.slint
--rw-r--r--   0     1001      127      332 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/exports/single_global_missing_export.slint
--rw-r--r--   0     1001      127      288 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/exports/unused_compo.slint
--rw-r--r--   0     1001      127     1464 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/expressions/arithmetic_op.slint
--rw-r--r--   0     1001      127     1261 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/expressions/clamp.slint
--rw-r--r--   0     1001      127      999 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/expressions/comparison_operator.slint
--rw-r--r--   0     1001      127     1473 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/expressions/condition_operator.slint
--rw-r--r--   0     1001      127     3442 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/expressions/image-url.slint
--rw-r--r--   0     1001      127     1090 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/expressions/image-url2.slint
--rw-r--r--   0     1001      127     1355 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/expressions/minmax.slint
--rw-r--r--   0     1001      127      654 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/expressions/percent2.slint
--rw-r--r--   0     1001      127      456 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/expressions/strings.slint
--rw-r--r--   0     1001      127     1221 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/expressions/unary_op.slint
--rw-r--r--   0     1001      127      387 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/focus/focus_invalid.slint
--rw-r--r--   0     1001      127     1078 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/focus/focus_not_called.slint
--rw-r--r--   0     1001      127      595 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/focus/focus_wrong_args.slint
--rw-r--r--   0     1001      127     1707 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/focus/initial_focus_non_input.slint
--rw-r--r--   0     1001      127      592 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/functions/function_double_qualified.slint
--rw-r--r--   0     1001      127     1814 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/functions/functions.slint
--rw-r--r--   0     1001      127     2990 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/functions/functions_call.slint
--rw-r--r--   0     1001      127     3353 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/functions/functions_purity.slint
--rw-r--r--   0     1001      127      597 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/imports/bug_2719.slint
--rw-r--r--   0     1001      127     1018 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/imports/bug_3674_alias-from-broken-import.slint
--rw-r--r--   0     1001      127      407 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/imports/cyclic_import.slint
--rw-r--r--   0     1001      127      441 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/imports/error_in_import.slint
--rw-r--r--   0     1001      127      252 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/imports/error_in_import2.slint
--rw-r--r--   0     1001      127      295 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/imports/error_in_import3.slint
--rw-r--r--   0     1001      127      410 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/imports/font.slint
--rw-r--r--   0     1001      127      393 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/imports/import_builtin.slint
--rw-r--r--   0     1001      127      411 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/imports/import_error2.slint
--rw-r--r--   0     1001      127      944 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/imports/import_errors.slint
--rw-r--r--   0     1001      127      207 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/imports/import_parse_error1.slint
--rw-r--r--   0     1001      127      221 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/imports/import_parse_error2.slint
--rw-r--r--   0     1001      127      238 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/imports/import_parse_error3.slint
--rw-r--r--   0     1001      127      239 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/imports/import_parse_error4.slint
--rw-r--r--   0     1001      127      503 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/imports/import_parse_error5.slint
--rw-r--r--   0     1001      127      472 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/imports/invalid_export.slint
--rw-r--r--   0     1001      127      379 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/imports/visibility_errors.slint
--rw-r--r--   0     1001      127      703 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/layout/if_in_grid.slint
--rw-r--r--   0     1001      127      441 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/layout/if_in_grid_row.slint
--rw-r--r--   0     1001      127      586 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/layout/min_max_conflict.slint
--rw-r--r--   0     1001      127      655 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/layout/spacing.slint
--rw-r--r--   0     1001      127      477 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/lookup/absolute-position.slint
--rw-r--r--   0     1001      127      691 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/lookup/array_index.slint
--rw-r--r--   0     1001      127      594 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/lookup/callback_alias.slint
--rw-r--r--   0     1001      127      641 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/lookup/callback_alias2.slint
--rw-r--r--   0     1001      127     1087 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/lookup/callback_alias3.slint
--rw-r--r--   0     1001      127      255 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/lookup/callback_alias_issue4938.slint
--rw-r--r--   0     1001      127      376 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/lookup/callback_not_called.slint
--rw-r--r--   0     1001      127      433 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/lookup/callback_return.slint
--rw-r--r--   0     1001      127     1814 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/lookup/color.slint
--rw-r--r--   0     1001      127     3112 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/lookup/conversion.slint
--rw-r--r--   0     1001      127     1807 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/lookup/dashes.slint
--rw-r--r--   0     1001      127     1250 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/lookup/deprecated_property.slint
--rw-r--r--   0     1001      127     1138 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/lookup/enum.slint
--rw-r--r--   0     1001      127     2598 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/lookup/for_lookup.slint
--rw-r--r--   0     1001      127     1211 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/lookup/global.slint
--rw-r--r--   0     1001      127      621 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/lookup/if.slint
--rw-r--r--   0     1001      127      920 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/lookup/issue_1461.slint
--rw-r--r--   0     1001      127     1287 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/lookup/property.slint
--rw-r--r--   0     1001      127     1704 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/lookup/recover_id_lookup.slint
--rw-r--r--   0     1001      127     1439 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/lookup/signal_arg.slint
--rw-r--r--   0     1001      127     1444 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/lookup/two_way_binding.slint
--rw-r--r--   0     1001      127     1220 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/lookup/two_way_binding_infer.slint
--rw-r--r--   0     1001      127      392 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/lookup/two_way_binding_model.slint
--rw-r--r--   0     1001      127      903 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/new_syntax/deprecated_syntax.slint
--rw-r--r--   0     1001      127     2695 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/new_syntax/input_output.slint
--rw-r--r--   0     1001      127     3062 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/new_syntax/input_output2.slint
--rw-r--r--   0     1001      127      593 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/new_syntax/new_component.slint
--rw-r--r--   0     1001      127     1020 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/new_syntax/new_lookup.slint
--rw-r--r--   0     1001      127     8651 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/new_syntax/two_way_input_output.slint
--rw-r--r--   0     1001      127      252 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/parse_error/children_placeholder0.slint
--rw-r--r--   0     1001      127      263 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/parse_error/export0.slint
--rw-r--r--   0     1001      127      219 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/parse_error/export1.slint
--rw-r--r--   0     1001      127      362 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/parse_error/if0.slint
--rw-r--r--   0     1001      127      278 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/parse_error/if1.slint
--rw-r--r--   0     1001      127      285 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/parse_error/if2.slint
--rw-r--r--   0     1001      127      224 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/parse_error/if3.slint
--rw-r--r--   0     1001      127      361 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/parse_error/if4.slint
--rw-r--r--   0     1001      127      398 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/parse_error/property1.slint
--rw-r--r--   0     1001      127      902 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/parse_error/property2.slint
--rw-r--r--   0     1001      127      846 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/parse_error/state1.slint
--rw-r--r--   0     1001      127      244 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/parse_error/state2.slint
--rw-r--r--   0     1001      127      307 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/parse_error/state3.slint
--rw-r--r--   0     1001      127      707 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax/parse_error/struct.slint
--rw-r--r--   0     1001      127     9426 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/syntax_tests.rs
--rw-r--r--   0     1001      127      156 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/typeloader/custom_style/TestStyle/std-widgets.slint
--rw-r--r--   0     1001      127      278 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/typeloader/dependency_local.slint
--rw-r--r--   0     1001      127      393 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/typeloader/dependency_test_main.slint
--rw-r--r--   0     1001      127      503 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/typeloader/incpath/bug_2719_import.slint
--rw-r--r--   0     1001      127      461 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/typeloader/incpath/bug_3674_alias_from_invalid_import.slint
--rw-r--r--   0     1001      127      262 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/typeloader/incpath/dependency_from_incpath.slint
--rw-r--r--   0     1001      127      205 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/typeloader/incpath/local_helper_type.slint
--rw-r--r--   0     1001      127      237 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/typeloader/incpath/should_fail.slint
--rw-r--r--   0     1001      127      320 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/typeloader/incpath/should_fail2.slint
--rw-r--r--   0     1001      127      280 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/typeloader/incpath/should_fail3.slint
--rw-r--r--   0     1001      127      491 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/typeloader/incpath/should_fail4.slint
--rw-r--r--   0     1001      127      208 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/typeloader/library/dependency_from_library.slint
--rw-r--r--   0     1001      127      243 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/typeloader/library/lib.slint
--rw-r--r--   0     1001      127      214 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/typeloader/library/library_helper_type.slint
--rw-r--r--   0     1001      127      324 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/typeloader/recursive_import1.slint
--rw-r--r--   0     1001      127      395 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/typeloader/recursive_import2.slint
--rw-r--r--   0     1001      127      450 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/tests/typeloader/some_rust_file.rs
--rw-r--r--   0     1001      127    43496 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/typeloader.rs
--rw-r--r--   0     1001      127    19576 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/typeregister.rs
--rw-r--r--   0     1001      127    14083 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/common/MadeWithSlint-logo-dark.svg
--rw-r--r--   0     1001      127    14073 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/common/MadeWithSlint-logo-light.svg
--rw-r--r--   0     1001      127     2358 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/common/combobox-base.slint
--rw-r--r--   0     1001      127     3861 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/common/common.slint
--rw-r--r--   0     1001      127     3184 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/common/lineedit-base.slint
--rw-r--r--   0     1001      127     4288 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/common/listview.slint
--rw-r--r--   0     1001      127     3920 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/common/slider-base.slint
--rw-r--r--   0     1001      127     2418 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/common/spinbox-base.slint
--rw-r--r--   0     1001      127     2510 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/common/spinner-base.slint
--rw-r--r--   0     1001      127     1202 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/common/standardbutton.slint
--rw-r--r--   0     1001      127     1080 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/common/tabwidget-base.slint
--rw-r--r--   0     1001      127      268 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic/color-scheme.slint
--rw-r--r--   0     1001      127      329 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic/std-widgets-impl.slint
--rw-r--r--   0     1001      127      212 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic/std-widgets.slint
--rw-r--r--   0     1001      127      308 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-base/_arrow_down.svg
--rw-r--r--   0     1001      127      284 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-base/_arrow_up.svg
--rw-r--r--   0     1001      127      413 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-base/_check-mark.svg
--rw-r--r--   0     1001      127      148 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-base/_pane_down.svg
--rw-r--r--   0     1001      127     2710 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-base/button.slint
--rw-r--r--   0     1001      127     2726 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-base/checkbox.slint
--rw-r--r--   0     1001      127     3057 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-base/combobox.slint
--rw-r--r--   0     1001      127     4437 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-base/components.slint
--rw-r--r--   0     1001      127     1000 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-base/groupbox.slint
--rw-r--r--   0     1001      127      632 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-base/layouts.slint
--rw-r--r--   0     1001      127     2886 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-base/lineedit.slint
--rw-r--r--   0     1001      127      988 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-base/progressindicator.slint
--rw-r--r--   0     1001      127     5065 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-base/scrollview.slint
--rw-r--r--   0     1001      127     2930 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-base/slider.slint
--rw-r--r--   0     1001      127     3327 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-base/spinbox.slint
--rw-r--r--   0     1001      127      733 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-base/spinner.slint
--rw-r--r--   0     1001      127     1524 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-base/std-widgets-base.slint
--rw-r--r--   0     1001      127     2126 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-base/std-widgets-impl.slint
--rw-r--r--   0     1001      127     3420 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-base/styling.slint
--rw-r--r--   0     1001      127     2861 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-base/switch.slint
--rw-r--r--   0     1001      127     9124 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-base/tableview.slint
--rw-r--r--   0     1001      127     6075 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-base/tabwidget.slint
--rw-r--r--   0     1001      127     4438 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-base/textedit.slint
--rw-r--r--   0     1001      127      257 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-dark/color-scheme.slint
--rw-r--r--   0     1001      127      329 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-dark/std-widgets-impl.slint
--rw-r--r--   0     1001      127      212 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-dark/std-widgets.slint
--rw-r--r--   0     1001      127      258 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-light/color-scheme.slint
--rw-r--r--   0     1001      127      329 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-light/std-widgets-impl.slint
--rw-r--r--   0     1001      127      212 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cosmic-light/std-widgets.slint
--rw-r--r--   0     1001      127      268 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino/color-scheme.slint
--rw-r--r--   0     1001      127      332 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino/std-widgets-impl.slint
--rw-r--r--   0     1001      127      215 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino/std-widgets.slint
--rw-r--r--   0     1001      127      513 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/_arrow-down.svg
--rw-r--r--   0     1001      127      507 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/_arrow-up.svg
--rw-r--r--   0     1001      127      780 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/_check-mark.svg
--rw-r--r--   0     1001      127      623 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/_chevron-down.svg
--rw-r--r--   0     1001      127      601 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/_chevron-up.svg
--rw-r--r--   0     1001      127      918 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/_down.svg
--rw-r--r--   0     1001      127      489 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/_dropdown.svg
--rw-r--r--   0     1001      127      849 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/_left.svg
--rw-r--r--   0     1001      127      815 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/_right.svg
--rw-r--r--   0     1001      127     1135 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/_up.svg
--rw-r--r--   0     1001      127     5134 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/button.slint
--rw-r--r--   0     1001      127     4547 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/checkbox.slint
--rw-r--r--   0     1001      127     5646 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/combobox.slint
--rw-r--r--   0     1001      127     3145 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/components.slint
--rw-r--r--   0     1001      127     1103 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/groupbox.slint
--rw-r--r--   0     1001      127      632 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/layouts.slint
--rw-r--r--   0     1001      127     3180 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/lineedit.slint
--rw-r--r--   0     1001      127     1404 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/progressindicator.slint
--rw-r--r--   0     1001      127     5563 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/scrollview.slint
--rw-r--r--   0     1001      127     3097 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/slider.slint
--rw-r--r--   0     1001      127     5483 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/spinbox.slint
--rw-r--r--   0     1001      127      739 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/spinner.slint
--rw-r--r--   0     1001      127     1524 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/std-widgets-base.slint
--rw-r--r--   0     1001      127     2216 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/std-widgets-impl.slint
--rw-r--r--   0     1001      127     4541 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/styling.slint
--rw-r--r--   0     1001      127     4097 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/switch.slint
--rw-r--r--   0     1001      127     8959 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/tableview.slint
--rw-r--r--   0     1001      127     5493 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/tabwidget.slint
--rw-r--r--   0     1001      127     6640 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-base/textedit.slint
--rw-r--r--   0     1001      127      257 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-dark/color-scheme.slint
--rw-r--r--   0     1001      127      332 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-dark/std-widgets-impl.slint
--rw-r--r--   0     1001      127      215 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-dark/std-widgets.slint
--rw-r--r--   0     1001      127      258 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-light/color-scheme.slint
--rw-r--r--   0     1001      127      332 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-light/std-widgets-impl.slint
--rw-r--r--   0     1001      127      215 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/cupertino-light/std-widgets.slint
--rw-r--r--   0     1001      127      268 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent/color-scheme.slint
--rw-r--r--   0     1001      127      329 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent/std-widgets-impl.slint
--rw-r--r--   0     1001      127      212 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent/std-widgets.slint
--rw-r--r--   0     1001      127      513 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/_arrow-down.svg
--rw-r--r--   0     1001      127      507 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/_arrow-up.svg
--rw-r--r--   0     1001      127      780 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/_check-mark.svg
--rw-r--r--   0     1001      127      623 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/_chevron-down.svg
--rw-r--r--   0     1001      127      601 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/_chevron-up.svg
--rw-r--r--   0     1001      127      918 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/_down.svg
--rw-r--r--   0     1001      127      489 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/_dropdown.svg
--rw-r--r--   0     1001      127      849 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/_left.svg
--rw-r--r--   0     1001      127      815 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/_right.svg
--rw-r--r--   0     1001      127     1135 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/_up.svg
--rw-r--r--   0     1001      127     4556 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/button.slint
--rw-r--r--   0     1001      127     3883 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/checkbox.slint
--rw-r--r--   0     1001      127     3773 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/combobox.slint
--rw-r--r--   0     1001      127     3363 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/components.slint
--rw-r--r--   0     1001      127      877 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/groupbox.slint
--rw-r--r--   0     1001      127      632 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/layouts.slint
--rw-r--r--   0     1001      127     3499 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/lineedit.slint
--rw-r--r--   0     1001      127     1023 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/progressindicator.slint
--rw-r--r--   0     1001      127     6590 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/scrollview.slint
--rw-r--r--   0     1001      127     3734 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/slider.slint
--rw-r--r--   0     1001      127     3992 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/spinbox.slint
--rw-r--r--   0     1001      127      733 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/spinner.slint
--rw-r--r--   0     1001      127     1524 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/std-widgets-base.slint
--rw-r--r--   0     1001      127     2126 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/std-widgets-impl.slint
--rw-r--r--   0     1001      127     6248 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/styling.slint
--rw-r--r--   0     1001      127     4616 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/switch.slint
--rw-r--r--   0     1001      127     9561 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/tableview.slint
--rw-r--r--   0     1001      127     5493 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/tabwidget.slint
--rw-r--r--   0     1001      127     4935 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-base/textedit.slint
--rw-r--r--   0     1001      127      257 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-dark/color-scheme.slint
--rw-r--r--   0     1001      127      329 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-dark/std-widgets-impl.slint
--rw-r--r--   0     1001      127      212 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-dark/std-widgets.slint
--rw-r--r--   0     1001      127      258 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-light/color-scheme.slint
--rw-r--r--   0     1001      127      329 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-light/std-widgets-impl.slint
--rw-r--r--   0     1001      127      212 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/fluent-light/std-widgets.slint
--rw-r--r--   0     1001      127      268 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material/color-scheme.slint
--rw-r--r--   0     1001      127      347 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material/std-widgets-impl.slint
--rw-r--r--   0     1001      127      214 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material/std-widgets.slint
--rw-r--r--   0     1001      127      163 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-base/_arrow-downward.svg
--rw-r--r--   0     1001      127      115 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-base/_arrow-drop-down.svg
--rw-r--r--   0     1001      127      115 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-base/_arrow-drop-up.svg
--rw-r--r--   0     1001      127      161 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-base/_arrow-upward.svg
--rw-r--r--   0     1001      127      150 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-base/_check-mark.svg
--rw-r--r--   0     1001      127      145 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-base/_expand-more.svg
--rw-r--r--   0     1001      127     3239 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-base/button.slint
--rw-r--r--   0     1001      127     5664 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-base/checkbox.slint
--rw-r--r--   0     1001      127     3452 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-base/combobox.slint
--rw-r--r--   0     1001      127     4712 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-base/components.slint
--rw-r--r--   0     1001      127     1477 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-base/groupbox.slint
--rw-r--r--   0     1001      127      633 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-base/layouts.slint
--rw-r--r--   0     1001      127     2866 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-base/lineedit.slint
--rw-r--r--   0     1001      127     1010 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-base/progressindicator.slint
--rw-r--r--   0     1001      127     5014 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-base/scrollview.slint
--rw-r--r--   0     1001      127     4146 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-base/slider.slint
--rw-r--r--   0     1001      127     5090 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-base/spinbox.slint
--rw-r--r--   0     1001      127      737 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-base/spinner.slint
--rw-r--r--   0     1001      127     1373 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-base/std-widgets-base.slint
--rw-r--r--   0     1001      127     2213 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-base/std-widgets-impl.slint
--rw-r--r--   0     1001      127     3651 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-base/styling.slint
--rw-r--r--   0     1001      127     6174 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-base/switch.slint
--rw-r--r--   0     1001      127     8186 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-base/tableview.slint
--rw-r--r--   0     1001      127     4886 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-base/tabwidget.slint
--rw-r--r--   0     1001      127      257 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-dark/color-scheme.slint
--rw-r--r--   0     1001      127      331 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-dark/std-widgets-impl.slint
--rw-r--r--   0     1001      127      214 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-dark/std-widgets.slint
--rw-r--r--   0     1001      127      258 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-light/color-scheme.slint
--rw-r--r--   0     1001      127      331 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-light/std-widgets-impl.slint
--rw-r--r--   0     1001      127      214 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/material-light/std-widgets.slint
--rw-r--r--   0     1001      127     1642 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/qt/button.slint
--rw-r--r--   0     1001      127      350 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/qt/checkbox.slint
--rw-r--r--   0     1001      127     1707 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/qt/combobox.slint
--rw-r--r--   0     1001      127      582 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/qt/groupbox.slint
--rw-r--r--   0     1001      127     2384 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/qt/internal-scrollview.slint
--rw-r--r--   0     1001      127      613 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/qt/layouts.slint
--rw-r--r--   0     1001      127     2377 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/qt/lineedit.slint
--rw-r--r--   0     1001      127      307 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/qt/progressindicator.slint
--rw-r--r--   0     1001      127     1026 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/qt/scrollview.slint
--rw-r--r--   0     1001      127      422 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/qt/slider.slint
--rw-r--r--   0     1001      127      834 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/qt/spinbox.slint
--rw-r--r--   0     1001      127     1265 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/qt/spinner.slint
--rw-r--r--   0     1001      127      374 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/qt/std-widgets-impl.slint
--rw-r--r--   0     1001      127     1475 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/qt/std-widgets.slint
--rw-r--r--   0     1001      127      346 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/qt/switch.slint
--rw-r--r--   0     1001      127     5310 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/qt/tableview.slint
--rw-r--r--   0     1001      127     1564 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/widgets/qt/tabwidget.slint
--rw-r--r--   0     1001      127     2855 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/renderers/skia/Cargo.toml
--rw-r--r--   0     1001      127    34670 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/renderers/skia/LICENSES/GPL-3.0-only.txt
--rw-r--r--   0     1001      127     3475 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/renderers/skia/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
--rw-r--r--   0     1001      127    14063 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/renderers/skia/LICENSES/LicenseRef-Slint-commercial.md
--rw-r--r--   0     1001      127      507 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/renderers/skia/README.md
--rw-r--r--   0     1001      127      673 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/renderers/skia/build.rs
--rw-r--r--   0     1001      127     6875 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/renderers/skia/cached_image.rs
--rw-r--r--   0     1001      127    14877 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/renderers/skia/d3d_surface.rs
--rw-r--r--   0     1001      127    34690 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/renderers/skia/itemrenderer.rs
--rw-r--r--   0     1001      127    23253 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/renderers/skia/lib.rs
--rw-r--r--   0     1001      127     6372 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/renderers/skia/metal_surface.rs
--rw-r--r--   0     1001      127    15370 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/renderers/skia/opengl_surface.rs
--rw-r--r--   0     1001      127     4611 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/renderers/skia/software_surface.rs
--rw-r--r--   0     1001      127    11843 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/renderers/skia/textlayout.rs
--rw-r--r--   0     1001      127    17420 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/renderers/skia/vulkan_surface.rs
--rw-r--r--   0     1001      127     9884 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/Cargo.toml
--rw-r--r--   0     1001      127    34670 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/LICENSES/GPL-3.0-only.txt
--rw-r--r--   0     1001      127     3475 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
--rw-r--r--   0     1001      127    14063 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/LICENSES/LicenseRef-Slint-commercial.md
--rw-r--r--   0     1001      127     1078 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/LICENSES/MIT.txt
--rw-r--r--   0     1001      127     1881 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/README.md
--rw-r--r--   0     1001      127     5140 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/android.rs
--rw-r--r--   0     1001      127      548 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/compile_fail_tests.rs
--rw-r--r--   0     1001      127     9447 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/building.md
--rw-r--r--   0     1001      127     7147 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/development.md
--rw-r--r--   0     1001      127     2881 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/install_qt.md
--rw-r--r--   0     1001      127        5 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/.gitignore
--rw-r--r--   0     1001      127     1013 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/README.md
--rw-r--r--   0     1001      127      261 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/book.toml
--rw-r--r--   0     1001      127      810 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/CMakeLists.txt
--rw-r--r--   0     1001      127      515 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/SUMMARY.md
--rw-r--r--   0     1001      127      268 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/appwindow.slint
--rw-r--r--   0     1001      127     1216 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/conclusion.md
--rw-r--r--   0     1001      127     1337 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/creating_the_tiles_from_cpp.md
--rw-r--r--   0     1001      127     2039 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/from_one_to_multiple_tiles.md
--rw-r--r--   0     1001      127     2483 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/game_logic_in_cpp.md
--rw-r--r--   0     1001      127     2126 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/getting_started.md
--rw-r--r--   0     1001      127      477 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/README.md
--rw-r--r--   0     1001      127     1122 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/at-solid.svg
--rw-r--r--   0     1001      127     3210 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/at.png
--rw-r--r--   0     1001      127      971 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/balance-scale-solid.svg
--rw-r--r--   0     1001      127     2265 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/balance-scale.png
--rw-r--r--   0     1001      127     1577 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/bicycle-solid.svg
--rw-r--r--   0     1001      127     2613 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/bicycle.png
--rw-r--r--   0     1001      127      837 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/bus-solid.svg
--rw-r--r--   0     1001      127     1540 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/bus.png
--rw-r--r--   0     1001      127      485 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/cloud-solid.svg
--rw-r--r--   0     1001      127     1454 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/cloud.png
--rw-r--r--   0     1001      127     2614 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/cogs-solid.svg
--rw-r--r--   0     1001      127     2894 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/cogs.png
--rw-r--r--   0     1001      127     1252 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/motorcycle-solid.svg
--rw-r--r--   0     1001      127     2497 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/motorcycle.png
--rw-r--r--   0     1001      127     6059 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/tile_logo.png
--rw-r--r--   0     1001      127      467 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/video-solid.svg
--rw-r--r--   0     1001      127     1073 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/video.png
--rw-r--r--   0     1001      127     1060 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/ideas_for_the_reader.md
--rw-r--r--   0     1001      127      953 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/introduction.md
--rw-r--r--   0     1001      127     2800 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/main_game_logic.cpp
--rw-r--r--   0     1001      127      300 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/main_initial.cpp
--rw-r--r--   0     1001      127      877 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/main_tiles_from_cpp.cpp
--rw-r--r--   0     1001      127     2620 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/memory_game_logic.slint
--rw-r--r--   0     1001      127     2130 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/memory_tile.md
--rw-r--r--   0     1001      127      425 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/memory_tile.slint
--rw-r--r--   0     1001      127     2205 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/memory_tiles_from_cpp.slint
--rw-r--r--   0     1001      127     2760 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/polishing_the_tile.md
--rw-r--r--   0     1001      127      262 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/book.toml
--rw-r--r--   0     1001      127      527 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/SUMMARY.md
--rw-r--r--   0     1001      127     1223 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/conclusion.md
--rw-r--r--   0     1001      127     1191 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/creating_the_tiles_from_js.md
--rw-r--r--   0     1001      127     2034 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/from_one_to_multiple_tiles.md
--rw-r--r--   0     1001      127     2031 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/game_logic_in_js.md
--rw-r--r--   0     1001      127     1515 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/getting_started.md
--rw-r--r--   0     1001      127      477 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/README.md
--rw-r--r--   0     1001      127     1122 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/at-solid.svg
--rw-r--r--   0     1001      127     3210 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/at.png
--rw-r--r--   0     1001      127      971 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/balance-scale-solid.svg
--rw-r--r--   0     1001      127     2265 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/balance-scale.png
--rw-r--r--   0     1001      127     1577 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/bicycle-solid.svg
--rw-r--r--   0     1001      127     2613 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/bicycle.png
--rw-r--r--   0     1001      127      837 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/bus-solid.svg
--rw-r--r--   0     1001      127     1540 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/bus.png
--rw-r--r--   0     1001      127      485 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/cloud-solid.svg
--rw-r--r--   0     1001      127     1454 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/cloud.png
--rw-r--r--   0     1001      127     2614 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/cogs-solid.svg
--rw-r--r--   0     1001      127     2894 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/cogs.png
--rw-r--r--   0     1001      127     1252 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/motorcycle-solid.svg
--rw-r--r--   0     1001      127     2497 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/motorcycle.png
--rw-r--r--   0     1001      127     6059 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/tile_logo.png
--rw-r--r--   0     1001      127      467 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/video-solid.svg
--rw-r--r--   0     1001      127     1073 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/video.png
--rw-r--r--   0     1001      127     1060 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/ideas_for_the_reader.md
--rw-r--r--   0     1001      127      960 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/introduction.md
--rw-r--r--   0     1001      127     1797 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/main_game_logic.js
--rw-r--r--   0     1001      127      275 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/main_initial.js
--rw-r--r--   0     1001      127      631 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/main_tiles_from_js.js
--rw-r--r--   0     1001      127      265 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/memory.slint
--rw-r--r--   0     1001      127     2620 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/memory_game_logic.slint
--rw-r--r--   0     1001      127     2079 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/memory_tile.md
--rw-r--r--   0     1001      127      425 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/memory_tile.slint
--rw-r--r--   0     1001      127     2205 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/memory_tiles_from_cpp.slint
--rw-r--r--   0     1001      127      202 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/package.json
--rw-r--r--   0     1001      127     2747 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/polishing_the_tile.md
--rw-r--r--   0     1001      127      262 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/rust/book.toml
--rw-r--r--   0     1001      127     3821 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/theme/head.hbs
--rw-r--r--   0     1001      127       84 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/theme/highlight.css
--rw-r--r--   0     1001      127      282 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/quickstart/theme/highlight.js
--rw-r--r--   0     1001      127      386 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/Pipfile
--rw-r--r--   0     1001      127      256 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/_static/theme_tweak.css
--rw-r--r--   0     1001      127      190 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/_templates/base.html
--rw-r--r--   0     1001      127     4339 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/conf.py
--rw-r--r--   0     1001      127      811 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/index.rst
--rw-r--r--   0     1001      127     7746 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/advanced/backend_linuxkms.md
--rw-r--r--   0     1001      127     1061 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/advanced/backend_qt.md
--rw-r--r--   0     1001      127     1692 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/advanced/backend_winit.md
--rw-r--r--   0     1001      127     7399 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/advanced/backends_and_renderers.md
--rw-r--r--   0     1001      127     6034 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/advanced/debugging_techniques.md
--rw-r--r--   0     1001      127     3816 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/advanced/style.md
--rw-r--r--   0     1001      127     1095 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/introduction/index.md
--rw-r--r--   0     1001      127     2287 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/introduction/supported_platforms.md
--rw-r--r--   0     1001      127     1418 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/builtins/callbacks.md
--rw-r--r--   0     1001      127    40679 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/builtins/elements.md
--rw-r--r--   0     1001      127      975 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/builtins/functions.md
--rw-r--r--   0     1001      127     3227 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/builtins/globals.md
--rw-r--r--   0     1001      127      267 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/builtins/index.rst
--rw-r--r--   0     1001      127     3567 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/builtins/namespaces.md
--rw-r--r--   0     1001      127     1144 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/concepts/container.md
--rw-r--r--   0     1001      127     2165 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/concepts/file.md
--rw-r--r--   0     1001      127     1591 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/concepts/focus.md
--rw-r--r--   0     1001      127     1232 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/concepts/fonts.md
--rw-r--r--   0     1001      127      262 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/concepts/index.rst
--rw-r--r--   0     1001      127    13939 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/concepts/layouting.md
--rw-r--r--   0     1001      127     1787 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/concepts/purity.md
--rw-r--r--   0     1001      127     7822 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/concepts/translations.md
--rw-r--r--   0     1001      127     2235 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/index.rst
--rw-r--r--   0     1001      127     2270 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/animations.md
--rw-r--r--   0     1001      127     1627 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/callbacks.md
--rw-r--r--   0     1001      127      326 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/comments.md
--rw-r--r--   0     1001      127      492 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/conditions.md
--rw-r--r--   0     1001      127     1792 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/expressions.md
--rw-r--r--   0     1001      127     1821 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/functions.md
--rw-r--r--   0     1001      127     2776 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/globals.md
--rw-r--r--   0     1001      127      413 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/identifiers.md
--rw-r--r--   0     1001      127      402 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/index.rst
--rw-r--r--   0     1001      127      851 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/legacy_syntax.md
--rw-r--r--   0     1001      127     3946 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/modules.md
--rw-r--r--   0     1001      127     5168 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/properties.md
--rw-r--r--   0     1001      127     1470 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/repetitions.md
--rw-r--r--   0     1001      127      658 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/statements.md
--rw-r--r--   0     1001      127     2210 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/states.md
--rw-r--r--   0     1001      127    17651 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/types.md
--rw-r--r--   0     1001      127      299 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/aboutslint.md
--rw-r--r--   0     1001      127     1469 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/button.md
--rw-r--r--   0     1001      127     1035 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/checkbox.md
--rw-r--r--   0     1001      127     1087 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/combobox.md
--rw-r--r--   0     1001      127      251 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/gridbox.md
--rw-r--r--   0     1001      127      741 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/groupbox.md
--rw-r--r--   0     1001      127      337 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/horizontalbox.md
--rw-r--r--   0     1001      127      569 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/index.rst
--rw-r--r--   0     1001      127     2305 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/lineedit.md
--rw-r--r--   0     1001      127     1293 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/listview.md
--rw-r--r--   0     1001      127      801 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/progressindicator.md
--rw-r--r--   0     1001      127     1976 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/scrollview.md
--rw-r--r--   0     1001      127     1120 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/slider.md
--rw-r--r--   0     1001      127      841 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/spinbox.md
--rw-r--r--   0     1001      127      805 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/spinner.md
--rw-r--r--   0     1001      127     1071 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/standardbutton.md
--rw-r--r--   0     1001      127     1489 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/standardlistview.md
--rw-r--r--   0     1001      127     2176 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/standardtableview.md
--rw-r--r--   0     1001      127     1037 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/switch.md
--rw-r--r--   0     1001      127      800 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/tabwidget.md
--rw-r--r--   0     1001      127     2146 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/textedit.md
--rw-r--r--   0     1001      127      335 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/verticalbox.md
--rw-r--r--   0     1001      127      565 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/widgets.md
--rw-r--r--   0     1001      127      364 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/recipes/button_native.slint
--rw-r--r--   0     1001      127    28191 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/reference/src/recipes/recipes.md
--rw-r--r--   0     1001      127     3821 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/resources/slint-docs-highlight.html
--rw-r--r--   0     1001      127     5521 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/resources/slint-docs-preview.html
--rw-r--r--   0     1001      127    13863 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/site/index.html
--rw-r--r--   0     1001      127     3880 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/testing.md
--rw-r--r--   0     1001      127     1698 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/torizon.md
--rw-r--r--   0     1001      127     3775 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs/triage.md
--rw-r--r--   0     1001      127     6705 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/docs.rs
--rw-r--r--   0     1001      127    14341 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/lib.rs
--rw-r--r--   0     1001      127    20004 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/mcu.md
--rw-r--r--   0     1001      127     7535 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/private_unstable_api.rs
--rw-r--r--   0     1001      127     8721 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/tests/partial_renderer.rs
--rw-r--r--   0     1001      127      889 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/tests/show_strongref.rs
--rw-r--r--   0     1001      127     1119 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/tests/simple_macro.rs
--rw-r--r--   0     1001      127     2490 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/tests/spawn_local.rs
--rw-r--r--   0     1001      127     2557 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/slint/type-mappings.md
--rw-r--r--   0     1001      127      706 2024-04-18 14:25:49.000000 slint-1.6.0a6/helper_crates/const-field-offset/macro/Cargo.toml
--rw-r--r--   0     1001      127    12200 2024-04-18 14:25:49.000000 slint-1.6.0a6/helper_crates/const-field-offset/macro/macro.rs
--rw-r--r--   0     1001      127      738 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/macros/Cargo.toml
--rw-r--r--   0     1001      127    34670 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/macros/LICENSES/GPL-3.0-only.txt
--rw-r--r--   0     1001      127     3475 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/macros/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
--rw-r--r--   0     1001      127    14063 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/macros/LICENSES/LicenseRef-Slint-commercial.md
--rw-r--r--   0     1001      127      507 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/macros/README.md
--rw-r--r--   0     1001      127    19345 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/macros/lib.rs
--rw-r--r--   0     1001      127      471 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/parser-test-macro/Cargo.toml
--rw-r--r--   0     1001      127      887 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/parser-test-macro/README.md
--rw-r--r--   0     1001      127     5619 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/compiler/parser-test-macro/lib.rs
--rw-r--r--   0     1001      127     1126 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/common/Cargo.toml
--rw-r--r--   0     1001      127    34670 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/common/LICENSES/GPL-3.0-only.txt
--rw-r--r--   0     1001      127     8815 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/common/LICENSES/LicenseRef-DejaVu-Font.txt
--rw-r--r--   0     1001      127     3475 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/common/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
--rw-r--r--   0     1001      127    14063 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/common/LICENSES/LicenseRef-Slint-commercial.md
--rw-r--r--   0     1001      127      635 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/common/README.md
--rw-r--r--   0     1001      127     7636 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/common/builtin_structs.rs
--rw-r--r--   0     1001      127    19223 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/common/enums.rs
--rw-r--r--   0     1001      127     8311 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/common/key_codes.rs
--rw-r--r--   0     1001      127     1322 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/common/lib.rs
--rw-r--r--   0     1001      127   757076 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/common/sharedfontdb/DejaVuSans.ttf
--rw-r--r--   0     1001      127      145 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/common/sharedfontdb/DejaVuSans.ttf.license
--rw-r--r--   0     1001      127     4526 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/common/sharedfontdb/fontconfig.rs
--rw-r--r--   0     1001      127     7491 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/common/sharedfontdb.rs
--rw-r--r--   0     1001      127     1109 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/android-activity/Cargo.toml
--rw-r--r--   0     1001      127    34670 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/android-activity/LICENSES/GPL-3.0-only.txt
--rw-r--r--   0     1001      127     3475 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/android-activity/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
--rw-r--r--   0     1001      127    14063 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/android-activity/LICENSES/LicenseRef-Slint-commercial.md
--rw-r--r--   0     1001      127      740 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/android-activity/README.md
--rw-r--r--   0     1001      127    34583 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/android-activity/androidwindowadapter.rs
--rw-r--r--   0     1001      127     4464 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/android-activity/build.rs
--rw-r--r--   0     1001      127    18055 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/android-activity/java/SlintAndroidJavaHelper.java
--rw-r--r--   0     1001      127    18156 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/android-activity/javahelper.rs
--rw-r--r--   0     1001      127     6133 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/android-activity/lib.rs
--rw-r--r--   0     1001      127     1955 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/linuxkms/Cargo.toml
--rw-r--r--   0     1001      127    34670 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/linuxkms/LICENSES/GPL-3.0-only.txt
--rw-r--r--   0     1001      127     3475 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/linuxkms/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
--rw-r--r--   0     1001      127    14063 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/linuxkms/LICENSES/LicenseRef-Slint-commercial.md
--rw-r--r--   0     1001      127     1078 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/linuxkms/LICENSES/MIT.txt
--rw-r--r--   0     1001      127      507 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/linuxkms/README.md
--rw-r--r--   0     1001      127    15614 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/linuxkms/calloop_backend/input.rs
--rw-r--r--   0     1001      127    12022 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/linuxkms/calloop_backend.rs
--rw-r--r--   0     1001      127     8655 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/linuxkms/display/gbmdisplay.rs
--rw-r--r--   0     1001      127     2955 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/linuxkms/display/swdisplay.rs
--rw-r--r--   0     1001      127     9345 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/linuxkms/display/vulkandisplay.rs
--rw-r--r--   0     1001      127     3237 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/linuxkms/display.rs
--rw-r--r--   0     1001      127    12140 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/linuxkms/drmoutput.rs
--rw-r--r--   0     1001      127     6253 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/linuxkms/fullscreenwindowadapter.rs
--rw-r--r--   0     1001      127     2022 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/linuxkms/lib.rs
--rw-r--r--   0     1001      127      365 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/linuxkms/mouse-pointer.svg
--rw-r--r--   0     1001      127      882 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/linuxkms/noop_backend.rs
--rw-r--r--   0     1001      127     7507 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/linuxkms/renderer/femtovg.rs
--rw-r--r--   0     1001      127     6654 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/linuxkms/renderer/skia.rs
--rw-r--r--   0     1001      127      532 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core-macros/Cargo.toml
--rw-r--r--   0     1001      127    34670 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core-macros/LICENSES/GPL-3.0-only.txt
--rw-r--r--   0     1001      127     3475 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core-macros/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
--rw-r--r--   0     1001      127    14063 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core-macros/LICENSES/LicenseRef-Slint-commercial.md
--rw-r--r--   0     1001      127      590 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core-macros/README.md
--rw-r--r--   0     1001      127     7310 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/core-macros/lib.rs
--rw-r--r--   0     1001      127     6405 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/interpreter/Cargo.toml
--rw-r--r--   0     1001      127    34670 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/interpreter/LICENSES/GPL-3.0-only.txt
--rw-r--r--   0     1001      127     3475 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/interpreter/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
--rw-r--r--   0     1001      127    14063 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/interpreter/LICENSES/LicenseRef-Slint-commercial.md
--rw-r--r--   0     1001      127    68116 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/interpreter/api.rs
--rw-r--r--   0     1001      127    83639 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/interpreter/dynamic_item_tree.rs
--rw-r--r--   0     1001      127     7555 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/interpreter/dynamic_type.rs
--rw-r--r--   0     1001      127    73407 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/interpreter/eval.rs
--rw-r--r--   0     1001      127    12240 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/interpreter/eval_layout.rs
--rw-r--r--   0     1001      127    31460 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/interpreter/ffi.rs
--rw-r--r--   0     1001      127     9875 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/interpreter/global_component.rs
--rw-r--r--   0     1001      127     5912 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/interpreter/highlight.rs
--rw-r--r--   0     1001      127     3015 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/interpreter/lib.rs
--rw-r--r--   0     1001      127     1425 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/interpreter/migration.rs
--rw-r--r--   0     1001      127     1795 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/interpreter/tests.rs
--rw-r--r--   0     1001      127     2301 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/interpreter/value_model.rs
--rw-r--r--   0     1001      127      571 2024-04-18 14:25:49.000000 slint-1.6.0a6/helper_crates/vtable/macro/Cargo.toml
--rw-r--r--   0     1001      127    10280 2024-04-18 14:25:49.000000 slint-1.6.0a6/helper_crates/vtable/macro/LICENSES/Apache-2.0.txt
--rw-r--r--   0     1001      127     1078 2024-04-18 14:25:49.000000 slint-1.6.0a6/helper_crates/vtable/macro/LICENSES/MIT.txt
--rw-r--r--   0     1001      127    31632 2024-04-18 14:25:49.000000 slint-1.6.0a6/helper_crates/vtable/macro/macro.rs
--rw-r--r--   0     1001      127     1383 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/Cargo.toml
--rw-r--r--   0     1001      127    34670 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/LICENSES/GPL-3.0-only.txt
--rw-r--r--   0     1001      127     3475 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
--rw-r--r--   0     1001      127    14063 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/LICENSES/LicenseRef-Slint-commercial.md
--rw-r--r--   0     1001      127      507 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/README.md
--rw-r--r--   0     1001      127    10783 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/accessible_generated.rs
--rw-r--r--   0     1001      127     2995 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/build.rs
--rw-r--r--   0     1001      127    27433 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/key_generated.rs
--rw-r--r--   0     1001      127    10534 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/lib.rs
--rw-r--r--   0     1001      127    32883 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/qt_accessible.rs
--rw-r--r--   0     1001      127    21040 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/qt_widgets/button.rs
--rw-r--r--   0     1001      127     6862 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/qt_widgets/checkbox.rs
--rw-r--r--   0     1001      127     9594 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/qt_widgets/combobox.rs
--rw-r--r--   0     1001      127     8992 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/qt_widgets/groupbox.rs
--rw-r--r--   0     1001      127     5930 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/qt_widgets/lineedit.rs
--rw-r--r--   0     1001      127     8178 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/qt_widgets/listviewitem.rs
--rw-r--r--   0     1001      127     7422 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/qt_widgets/palette.rs
--rw-r--r--   0     1001      127     4945 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/qt_widgets/progress_indicator.rs
--rw-r--r--   0     1001      127    19794 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/qt_widgets/scrollview.rs
--rw-r--r--   0     1001      127    13934 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/qt_widgets/slider.rs
--rw-r--r--   0     1001      127    12529 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/qt_widgets/spinbox.rs
--rw-r--r--   0     1001      127     8594 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/qt_widgets/stylemetrics.rs
--rw-r--r--   0     1001      127     5637 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/qt_widgets/tableheadersection.rs
--rw-r--r--   0     1001      127    22411 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/qt_widgets/tabwidget.rs
--rw-r--r--   0     1001      127    12967 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/qt_widgets.rs
--rw-r--r--   0     1001      127   103898 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/qt/qt_window.rs
--rw-r--r--   0     1001      127     1919 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/renderers/femtovg/Cargo.toml
--rw-r--r--   0     1001      127    34670 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/renderers/femtovg/LICENSES/GPL-3.0-only.txt
--rw-r--r--   0     1001      127     3475 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/renderers/femtovg/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
--rw-r--r--   0     1001      127    14063 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/renderers/femtovg/LICENSES/LicenseRef-Slint-commercial.md
--rw-r--r--   0     1001      127      507 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/renderers/femtovg/README.md
--rw-r--r--   0     1001      127    26501 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/renderers/femtovg/fonts.rs
--rw-r--r--   0     1001      127     9732 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/renderers/femtovg/images.rs
--rw-r--r--   0     1001      127    60402 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/renderers/femtovg/itemrenderer.rs
--rw-r--r--   0     1001      127    23205 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/renderers/femtovg/lib.rs
--rw-r--r--   0     1001      127      603 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/testing/Cargo.toml
--rw-r--r--   0     1001      127      507 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/testing/README.md
--rw-r--r--   0     1001      127    10886 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/testing/lib.rs
--rw-r--r--   0     1001      127      623 2024-04-18 14:25:49.000000 slint-1.6.0a6/helper_crates/vtable/Cargo.toml
--rw-r--r--   0     1001      127     1796 2024-04-18 14:25:49.000000 slint-1.6.0a6/helper_crates/vtable/CHANGELOG.md
--rw-r--r--   0     1001      127    10280 2024-04-18 14:25:49.000000 slint-1.6.0a6/helper_crates/vtable/LICENSES/Apache-2.0.txt
--rw-r--r--   0     1001      127     1078 2024-04-18 14:25:49.000000 slint-1.6.0a6/helper_crates/vtable/LICENSES/MIT.txt
--rw-r--r--   0     1001      127      399 2024-04-18 14:25:49.000000 slint-1.6.0a6/helper_crates/vtable/README.md
--rw-r--r--   0     1001      127     3723 2024-04-18 14:25:49.000000 slint-1.6.0a6/helper_crates/vtable/src/compile_fail_tests.rs
--rw-r--r--   0     1001      127    18776 2024-04-18 14:25:49.000000 slint-1.6.0a6/helper_crates/vtable/src/lib.rs
--rw-r--r--   0     1001      127    18973 2024-04-18 14:25:49.000000 slint-1.6.0a6/helper_crates/vtable/src/vrc.rs
--rw-r--r--   0     1001      127     9552 2024-04-18 14:25:49.000000 slint-1.6.0a6/helper_crates/vtable/tests/test_vrc.rs
--rw-r--r--   0     1001      127     5359 2024-04-18 14:25:49.000000 slint-1.6.0a6/helper_crates/vtable/tests/test_vtable.rs
--rw-r--r--   0     1001      127      768 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/build/Cargo.toml
--rw-r--r--   0     1001      127    34670 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/build/LICENSES/GPL-3.0-only.txt
--rw-r--r--   0     1001      127     3475 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/build/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
--rw-r--r--   0     1001      127    14063 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/build/LICENSES/LicenseRef-Slint-commercial.md
--rw-r--r--   0     1001      127    15366 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/rs/build/lib.rs
--rw-r--r--   0     1001      127     2370 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/selector/Cargo.toml
--rw-r--r--   0     1001      127    34670 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/selector/LICENSES/GPL-3.0-only.txt
--rw-r--r--   0     1001      127     3475 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/selector/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
--rw-r--r--   0     1001      127    14063 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/selector/LICENSES/LicenseRef-Slint-commercial.md
--rw-r--r--   0     1001      127      872 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/selector/README.md
--rw-r--r--   0     1001      127     2014 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/selector/build.rs
--rw-r--r--   0     1001      127     5859 2024-04-18 14:25:49.000000 slint-1.6.0a6/internal/backends/selector/lib.rs
--rw-r--r--   0     1001      127      630 2024-04-18 14:25:49.000000 slint-1.6.0a6/helper_crates/const-field-offset/Cargo.toml
--rw-r--r--   0     1001      127      610 2024-04-18 14:25:49.000000 slint-1.6.0a6/helper_crates/const-field-offset/CHANGELOG.md
--rw-r--r--   0     1001      127    10280 2024-04-18 14:25:49.000000 slint-1.6.0a6/helper_crates/const-field-offset/LICENSES/Apache-2.0.txt
--rw-r--r--   0     1001      127     1078 2024-04-18 14:25:49.000000 slint-1.6.0a6/helper_crates/const-field-offset/LICENSES/MIT.txt
--rw-r--r--   0     1001      127      492 2024-04-18 14:25:49.000000 slint-1.6.0a6/helper_crates/const-field-offset/README.md
--rw-r--r--   0     1001      127     6982 2024-04-18 14:25:49.000000 slint-1.6.0a6/helper_crates/const-field-offset/src/lib.rs
--rw-r--r--   0     1001      127     4766 2024-04-18 14:25:49.000000 slint-1.6.0a6/helper_crates/const-field-offset/tests/test_field_offset.rs
--rw-r--r--   0        0        0      931 1970-01-01 00:00:00.000000 slint-1.6.0a6/api/python/Cargo.toml
--rw-r--r--   0     1001      127       11 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/python/.gitignore
--rw-r--r--   0     1001      127     7668 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/python/README.md
--rw-r--r--   0     1001      127     4367 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/python/brush.rs
--rw-r--r--   0     1001      127     3303 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/python/errors.rs
--rw-r--r--   0     1001      127     1399 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/python/image.rs
--rw-r--r--   0     1001      127    10939 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/python/interpreter.rs
--rw-r--r--   0     1001      127     1421 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/python/lib.rs
--rw-r--r--   0     1001      127     6300 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/python/models.rs
--rw-r--r--   0     1001      127      348 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/python/noxfile.py
--rw-r--r--   0     1001      127     7729 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/python/slint/__init__.py
--rw-r--r--   0     1001      127     1889 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/python/slint/models.py
--rw-r--r--   0     1001      127     1164 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/python/tests/test_brush.py
--rw-r--r--   0     1001      127     1019 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/python/tests/test_callback_decorators.py
--rw-r--r--   0     1001      127     2369 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/python/tests/test_compiler.py
--rw-r--r--   0     1001      127     1095 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/python/tests/test_gc.py
--rw-r--r--   0     1001      127     6577 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/python/tests/test_instance.py
--rw-r--r--   0     1001      127     1597 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/python/tests/test_load_file.py
--rw-r--r--   0     1001      127      905 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/python/tests/test_load_file.slint
--rw-r--r--   0     1001      127      687 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/python/tests/test_loader.py
--rw-r--r--   0     1001      127     3589 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/python/tests/test_models.py
--rw-r--r--   0     1001      127      832 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/python/tests/test_timers.py
--rw-r--r--   0     1001      127     2403 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/python/timer.rs
--rw-r--r--   0     1001      127     4717 2024-04-18 14:25:49.000000 slint-1.6.0a6/api/python/value.rs
--rw-r--r--   0     1001      127   207085 2024-04-18 14:25:54.000000 slint-1.6.0a6/Cargo.lock
--rw-r--r--   0        0        0     4140 1970-01-01 00:00:00.000000 slint-1.6.0a6/Cargo.toml
--rw-r--r--   0        0        0     1487 1970-01-01 00:00:00.000000 slint-1.6.0a6/pyproject.toml
--rw-r--r--   0     1001      127     7729 2024-04-18 14:25:49.000000 slint-1.6.0a6/slint/__init__.py
--rw-r--r--   0     1001      127     1889 2024-04-18 14:25:49.000000 slint-1.6.0a6/slint/models.py
--rw-r--r--   0        0        0     9215 1970-01-01 00:00:00.000000 slint-1.6.0a6/PKG-INFO
+-rw-r--r--   0     1001      127      738 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/macros/Cargo.toml
+-rw-r--r--   0     1001      127    34670 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/macros/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0     1001      127     3475 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/macros/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
+-rw-r--r--   0     1001      127    14063 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/macros/LICENSES/LicenseRef-Slint-commercial.md
+-rw-r--r--   0     1001      127      507 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/macros/README.md
+-rw-r--r--   0     1001      127    19345 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/macros/lib.rs
+-rw-r--r--   0     1001      127     1955 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/linuxkms/Cargo.toml
+-rw-r--r--   0     1001      127    34670 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/linuxkms/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0     1001      127     3475 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/linuxkms/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
+-rw-r--r--   0     1001      127    14063 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/linuxkms/LICENSES/LicenseRef-Slint-commercial.md
+-rw-r--r--   0     1001      127     1078 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/linuxkms/LICENSES/MIT.txt
+-rw-r--r--   0     1001      127      507 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/linuxkms/README.md
+-rw-r--r--   0     1001      127    15614 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/linuxkms/calloop_backend/input.rs
+-rw-r--r--   0     1001      127    11770 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/linuxkms/calloop_backend.rs
+-rw-r--r--   0     1001      127     8655 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/linuxkms/display/gbmdisplay.rs
+-rw-r--r--   0     1001      127     2955 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/linuxkms/display/swdisplay.rs
+-rw-r--r--   0     1001      127     9345 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/linuxkms/display/vulkandisplay.rs
+-rw-r--r--   0     1001      127     3237 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/linuxkms/display.rs
+-rw-r--r--   0     1001      127    11904 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/linuxkms/drmoutput.rs
+-rw-r--r--   0     1001      127     6253 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/linuxkms/fullscreenwindowadapter.rs
+-rw-r--r--   0     1001      127     2022 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/linuxkms/lib.rs
+-rw-r--r--   0     1001      127      365 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/linuxkms/mouse-pointer.svg
+-rw-r--r--   0     1001      127      882 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/linuxkms/noop_backend.rs
+-rw-r--r--   0     1001      127     7507 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/linuxkms/renderer/femtovg.rs
+-rw-r--r--   0     1001      127     6654 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/linuxkms/renderer/skia.rs
+-rw-r--r--   0     1001      127     1913 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/Cargo.toml
+-rw-r--r--   0     1001      127    10280 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/LICENSES/Apache-2.0.txt
+-rw-r--r--   0     1001      127    16830 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/LICENSES/CC-BY-ND-4.0.txt
+-rw-r--r--   0     1001      127    34670 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0     1001      127     3475 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
+-rw-r--r--   0     1001      127    14063 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/LICENSES/LicenseRef-Slint-commercial.md
+-rw-r--r--   0     1001      127     1078 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/LICENSES/MIT.txt
+-rw-r--r--   0     1001      127      537 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/README.md
+-rw-r--r--   0     1001      127     2420 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/build.rs
+-rw-r--r--   0     1001      127    16358 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/builtin_macros.rs
+-rw-r--r--   0     1001      127    18500 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/builtins.slint
+-rw-r--r--   0     1001      127    19681 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/diagnostics.rs
+-rw-r--r--   0     1001      127     2636 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/embedded_resources.rs
+-rw-r--r--   0     1001      127    69892 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/expression_tree.rs
+-rw-r--r--   0     1001      127     4420 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/fileaccess.rs
+-rw-r--r--   0     1001      127   141177 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/generator/cpp.rs
+-rw-r--r--   0     1001      127   123809 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/generator/rust.rs
+-rw-r--r--   0     1001      127    19509 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/generator.rs
+-rw-r--r--   0     1001      127    32752 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/langtype.rs
+-rw-r--r--   0     1001      127    21425 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/layout.rs
+-rw-r--r--   0     1001      127    15374 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/lexer.rs
+-rw-r--r--   0     1001      127     9358 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/lib.rs
+-rw-r--r--   0     1001      127     7020 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/literals.rs
+-rw-r--r--   0     1001      127    31386 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/llr/expression.rs
+-rw-r--r--   0     1001      127    13532 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/llr/item_tree.rs
+-rw-r--r--   0     1001      127    40541 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/llr/lower_expression.rs
+-rw-r--r--   0     1001      127    31938 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/llr/lower_to_item_tree.rs
+-rw-r--r--   0     1001      127     6503 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/llr/optim_passes/count_property_use.rs
+-rw-r--r--   0     1001      127     6269 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/llr/optim_passes/inline_expressions.rs
+-rw-r--r--   0     1001      127    11380 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/llr/pretty_print.rs
+-rw-r--r--   0     1001      127      654 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/llr.rs
+-rw-r--r--   0     1001      127    11758 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/load_builtins.rs
+-rw-r--r--   0     1001      127    39783 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/lookup.rs
+-rw-r--r--   0     1001      127     7518 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/namedreference.rs
+-rw-r--r--   0     1001      127   103277 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/object_tree.rs
+-rw-r--r--   0     1001      127    10913 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/parser/document.rs
+-rw-r--r--   0     1001      127    21286 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/parser/element.rs
+-rw-r--r--   0     1001      127    14696 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/parser/expressions.rs
+-rw-r--r--   0     1001      127     3102 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/parser/statements.rs
+-rw-r--r--   0     1001      127     4561 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/parser/type.rs
+-rw-r--r--   0     1001      127    36378 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/parser.rs
+-rw-r--r--   0     1001      127     3949 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/apply_default_properties_from_style.rs
+-rw-r--r--   0     1001      127    22379 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/binding_analysis.rs
+-rw-r--r--   0     1001      127     1587 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/border_radius.rs
+-rw-r--r--   0     1001      127     1793 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/check_expressions.rs
+-rw-r--r--   0     1001      127     1941 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/check_public_api.rs
+-rw-r--r--   0     1001      127     2309 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/check_rotation.rs
+-rw-r--r--   0     1001      127     4580 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/clip.rs
+-rw-r--r--   0     1001      127     2464 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/collect_custom_fonts.rs
+-rw-r--r--   0     1001      127     1933 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/collect_globals.rs
+-rw-r--r--   0     1001      127     1150 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/collect_init_code.rs
+-rw-r--r--   0     1001      127     4172 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/collect_structs_and_enums.rs
+-rw-r--r--   0     1001      127     1690 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/collect_subcomponents.rs
+-rw-r--r--   0     1001      127     8043 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/compile_paths.rs
+-rw-r--r--   0     1001      127     9466 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/const_propagation.rs
+-rw-r--r--   0     1001      127     6155 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/deduplicate_property_read.rs
+-rw-r--r--   0     1001      127    18877 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/default_geometry.rs
+-rw-r--r--   0     1001      127    16260 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/embed_glyphs.rs
+-rw-r--r--   0     1001      127    14883 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/embed_images.rs
+-rw-r--r--   0     1001      127     5157 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/ensure_window.rs
+-rw-r--r--   0     1001      127     6270 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/flickable.rs
+-rw-r--r--   0     1001      127    11618 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/focus_handling.rs
+-rw-r--r--   0     1001      127     4318 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/generate_item_indices.rs
+-rw-r--r--   0     1001      127     6709 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/infer_aliases_types.rs
+-rw-r--r--   0     1001      127    21455 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/inlining.rs
+-rw-r--r--   0     1001      127     3241 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/lower_absolute_coordinates.rs
+-rw-r--r--   0     1001      127     3268 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/lower_accessibility.rs
+-rw-r--r--   0     1001      127     1697 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/lower_component_container.rs
+-rw-r--r--   0     1001      127    31672 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/lower_layout.rs
+-rw-r--r--   0     1001      127     5565 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/lower_popups.rs
+-rw-r--r--   0     1001      127     5182 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/lower_property_to_element.rs
+-rw-r--r--   0     1001      127     6916 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/lower_shadows.rs
+-rw-r--r--   0     1001      127     9988 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/lower_states.rs
+-rw-r--r--   0     1001      127     8355 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/lower_tabwidget.rs
+-rw-r--r--   0     1001      127     2000 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/lower_text_input_interface.rs
+-rw-r--r--   0     1001      127     6185 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/materialize_fake_properties.rs
+-rw-r--r--   0     1001      127     7514 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/move_declarations.rs
+-rw-r--r--   0     1001      127     2749 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/optimize_useless_rectangles.rs
+-rw-r--r--   0     1001      127     4231 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/purity_check.rs
+-rw-r--r--   0     1001      127     9197 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/remove_aliases.rs
+-rw-r--r--   0     1001      127    19427 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/remove_return.rs
+-rw-r--r--   0     1001      127     1656 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/remove_unused_properties.rs
+-rw-r--r--   0     1001      127     5145 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/repeater_component.rs
+-rw-r--r--   0     1001      127     5620 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/resolve_native_classes.rs
+-rw-r--r--   0     1001      127    71031 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/resolving.rs
+-rw-r--r--   0     1001      127     3046 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/unique_id.rs
+-rw-r--r--   0     1001      127     4210 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/visible.rs
+-rw-r--r--   0     1001      127     2961 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/z_order.rs
+-rw-r--r--   0     1001      127    10741 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes.rs
+-rw-r--r--   0     1001      127    18378 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/pathutils.rs
+-rw-r--r--   0     1001      127     8812 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/consistent_styles.rs
+-rw-r--r--   0     1001      127     1237 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/accessibility/accessible_properties.slint
+-rw-r--r--   0     1001      127     1774 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/analysis/binding_loop1.slint
+-rw-r--r--   0     1001      127     1826 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/analysis/binding_loop2.slint
+-rw-r--r--   0     1001      127      924 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/analysis/binding_loop_function.slint
+-rw-r--r--   0     1001      127      643 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/analysis/binding_loop_issue_772.slint
+-rw-r--r--   0     1001      127     2458 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/analysis/binding_loop_layout.slint
+-rw-r--r--   0     1001      127     1854 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/analysis/binding_loop_layout2.slint
+-rw-r--r--   0     1001      127     1144 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/analysis/binding_loop_layout3.slint
+-rw-r--r--   0     1001      127     2120 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/analysis/binding_loop_layout4.slint
+-rw-r--r--   0     1001      127      488 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/analysis/binding_loop_mappointtowindow.slint
+-rw-r--r--   0     1001      127      923 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/analysis/binding_loop_self.slint
+-rw-r--r--   0     1001      127      942 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/animate.slint
+-rw-r--r--   0     1001      127      230 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/array.slint
+-rw-r--r--   0     1001      127      788 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/assign.slint
+-rw-r--r--   0     1001      127      585 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/box_shadow.slint
+-rw-r--r--   0     1001      127     1021 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/children_placeholder.slint
+-rw-r--r--   0     1001      127      301 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/children_placeholder_2.slint
+-rw-r--r--   0     1001      127      663 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/clip.slint
+-rw-r--r--   0     1001      127      492 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/comments.slint
+-rw-r--r--   0     1001      127     2078 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/dialog.slint
+-rw-r--r--   0     1001      127      631 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/dialog2.slint
+-rw-r--r--   0     1001      127      499 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/double_binding.slint
+-rw-r--r--   0     1001      127      270 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/double_color.slint
+-rw-r--r--   0     1001      127     1137 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/duplicated_id.slint
+-rw-r--r--   0     1001      127     1340 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/easing.slint
+-rw-r--r--   0     1001      127      383 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/easing_not_called.slint
+-rw-r--r--   0     1001      127      156 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/empty.slint
+-rw-r--r--   0     1001      127      526 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/enums.slint
+-rw-r--r--   0     1001      127      441 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/for.slint
+-rw-r--r--   0     1001      127      492 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/image.slint
+-rw-r--r--   0     1001      127      450 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/inline_component.slint
+-rw-r--r--   0     1001      127      895 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/item_as_property.slint
+-rw-r--r--   0     1001      127      465 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/layout.slint
+-rw-r--r--   0     1001      127     1958 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/layout2.slint
+-rw-r--r--   0     1001      127     2188 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/linear-gradient.slint
+-rw-r--r--   0     1001      127      470 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/object_in_binding.slint
+-rw-r--r--   0     1001      127      538 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/opacity.slint
+-rw-r--r--   0     1001      127      905 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/parse_error.slint
+-rw-r--r--   0     1001      127      535 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/path.slint
+-rw-r--r--   0     1001      127     1114 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/path_commands.slint
+-rw-r--r--   0     1001      127      541 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/path_for.slint
+-rw-r--r--   0     1001      127     1056 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/percent.slint
+-rw-r--r--   0     1001      127      707 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/popup.slint
+-rw-r--r--   0     1001      127      333 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/property_animation.slint
+-rw-r--r--   0     1001      127      983 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/property_declaration.slint
+-rw-r--r--   0     1001      127      268 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/property_declaration_in_component.slint
+-rw-r--r--   0     1001      127     1786 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/radial-gradient.slint
+-rw-r--r--   0     1001      127      837 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/return.slint
+-rw-r--r--   0     1001      127     1850 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/rotation.slint
+-rw-r--r--   0     1001      127      456 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/rust-attr.slint
+-rw-r--r--   0     1001      127     1781 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/self_assign.slint
+-rw-r--r--   0     1001      127     1413 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/signal.slint
+-rw-r--r--   0     1001      127     4436 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/states_transitions.slint
+-rw-r--r--   0     1001      127      711 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/states_transitions2.slint
+-rw-r--r--   0     1001      127      748 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/states_transitions3.slint
+-rw-r--r--   0     1001      127      731 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/states_two_way.slint
+-rw-r--r--   0     1001      127      731 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/sub_elements.slint
+-rw-r--r--   0     1001      127      218 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/supersimple.slint
+-rw-r--r--   0     1001      127      467 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/svg_path.slint
+-rw-r--r--   0     1001      127     1600 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/tr.slint
+-rw-r--r--   0     1001      127     3038 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/tr2.slint
+-rw-r--r--   0     1001      127     1108 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/type_declaration.slint
+-rw-r--r--   0     1001      127     1391 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/unknown_item.slint
+-rw-r--r--   0     1001      127      457 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/callbacks/init.slint
+-rw-r--r--   0     1001      127      552 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/callbacks/property-changes.slint
+-rw-r--r--   0     1001      127      671 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/elements/component_container.slint
+-rw-r--r--   0     1001      127     1202 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/elements/listview.slint
+-rw-r--r--   0     1001      127      601 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/elements/popup.slint
+-rw-r--r--   0     1001      127      538 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/elements/tabwidget.slint
+-rw-r--r--   0     1001      127      898 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/elements/tabwidget2.slint
+-rw-r--r--   0     1001      127      474 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/elements/tabwidget3.slint
+-rw-r--r--   0     1001      127      436 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/exports/export_duplicates.slint
+-rw-r--r--   0     1001      127      623 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/exports/reexport_duplicate.slint
+-rw-r--r--   0     1001      127      326 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/exports/root_compo_export.slint
+-rw-r--r--   0     1001      127      289 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/exports/root_compo_export2.slint
+-rw-r--r--   0     1001      127      332 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/exports/single_global_missing_export.slint
+-rw-r--r--   0     1001      127      288 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/exports/unused_compo.slint
+-rw-r--r--   0     1001      127     1464 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/expressions/arithmetic_op.slint
+-rw-r--r--   0     1001      127     1261 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/expressions/clamp.slint
+-rw-r--r--   0     1001      127      999 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/expressions/comparison_operator.slint
+-rw-r--r--   0     1001      127     1473 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/expressions/condition_operator.slint
+-rw-r--r--   0     1001      127     3442 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/expressions/image-url.slint
+-rw-r--r--   0     1001      127     1090 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/expressions/image-url2.slint
+-rw-r--r--   0     1001      127     1355 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/expressions/minmax.slint
+-rw-r--r--   0     1001      127      654 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/expressions/percent2.slint
+-rw-r--r--   0     1001      127      456 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/expressions/strings.slint
+-rw-r--r--   0     1001      127     1221 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/expressions/unary_op.slint
+-rw-r--r--   0     1001      127      387 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/focus/focus_invalid.slint
+-rw-r--r--   0     1001      127     1078 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/focus/focus_not_called.slint
+-rw-r--r--   0     1001      127      705 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/focus/focus_wrong_args.slint
+-rw-r--r--   0     1001      127     1707 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/focus/initial_focus_non_input.slint
+-rw-r--r--   0     1001      127      592 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/functions/function_double_qualified.slint
+-rw-r--r--   0     1001      127     1814 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/functions/functions.slint
+-rw-r--r--   0     1001      127     2990 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/functions/functions_call.slint
+-rw-r--r--   0     1001      127     3353 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/functions/functions_purity.slint
+-rw-r--r--   0     1001      127      597 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/imports/bug_2719.slint
+-rw-r--r--   0     1001      127     1018 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/imports/bug_3674_alias-from-broken-import.slint
+-rw-r--r--   0     1001      127      407 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/imports/cyclic_import.slint
+-rw-r--r--   0     1001      127      441 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/imports/error_in_import.slint
+-rw-r--r--   0     1001      127      252 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/imports/error_in_import2.slint
+-rw-r--r--   0     1001      127      295 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/imports/error_in_import3.slint
+-rw-r--r--   0     1001      127      410 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/imports/font.slint
+-rw-r--r--   0     1001      127      393 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/imports/import_builtin.slint
+-rw-r--r--   0     1001      127      411 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/imports/import_error2.slint
+-rw-r--r--   0     1001      127      944 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/imports/import_errors.slint
+-rw-r--r--   0     1001      127      207 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/imports/import_parse_error1.slint
+-rw-r--r--   0     1001      127      221 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/imports/import_parse_error2.slint
+-rw-r--r--   0     1001      127      238 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/imports/import_parse_error3.slint
+-rw-r--r--   0     1001      127      239 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/imports/import_parse_error4.slint
+-rw-r--r--   0     1001      127      503 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/imports/import_parse_error5.slint
+-rw-r--r--   0     1001      127      472 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/imports/invalid_export.slint
+-rw-r--r--   0     1001      127      379 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/imports/visibility_errors.slint
+-rw-r--r--   0     1001      127      703 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/layout/if_in_grid.slint
+-rw-r--r--   0     1001      127      441 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/layout/if_in_grid_row.slint
+-rw-r--r--   0     1001      127      586 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/layout/min_max_conflict.slint
+-rw-r--r--   0     1001      127      655 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/layout/spacing.slint
+-rw-r--r--   0     1001      127      477 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/lookup/absolute-position.slint
+-rw-r--r--   0     1001      127      691 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/lookup/array_index.slint
+-rw-r--r--   0     1001      127      594 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/lookup/callback_alias.slint
+-rw-r--r--   0     1001      127      641 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/lookup/callback_alias2.slint
+-rw-r--r--   0     1001      127     1087 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/lookup/callback_alias3.slint
+-rw-r--r--   0     1001      127      255 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/lookup/callback_alias_issue4938.slint
+-rw-r--r--   0     1001      127      376 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/lookup/callback_not_called.slint
+-rw-r--r--   0     1001      127      433 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/lookup/callback_return.slint
+-rw-r--r--   0     1001      127     1814 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/lookup/color.slint
+-rw-r--r--   0     1001      127     3112 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/lookup/conversion.slint
+-rw-r--r--   0     1001      127     1807 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/lookup/dashes.slint
+-rw-r--r--   0     1001      127     1250 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/lookup/deprecated_property.slint
+-rw-r--r--   0     1001      127     1138 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/lookup/enum.slint
+-rw-r--r--   0     1001      127     2598 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/lookup/for_lookup.slint
+-rw-r--r--   0     1001      127     1211 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/lookup/global.slint
+-rw-r--r--   0     1001      127      621 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/lookup/if.slint
+-rw-r--r--   0     1001      127      920 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/lookup/issue_1461.slint
+-rw-r--r--   0     1001      127     1287 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/lookup/property.slint
+-rw-r--r--   0     1001      127     1704 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/lookup/recover_id_lookup.slint
+-rw-r--r--   0     1001      127     1439 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/lookup/signal_arg.slint
+-rw-r--r--   0     1001      127     1444 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/lookup/two_way_binding.slint
+-rw-r--r--   0     1001      127     1220 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/lookup/two_way_binding_infer.slint
+-rw-r--r--   0     1001      127      392 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/lookup/two_way_binding_model.slint
+-rw-r--r--   0     1001      127      903 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/new_syntax/deprecated_syntax.slint
+-rw-r--r--   0     1001      127     2695 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/new_syntax/input_output.slint
+-rw-r--r--   0     1001      127     3062 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/new_syntax/input_output2.slint
+-rw-r--r--   0     1001      127      593 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/new_syntax/new_component.slint
+-rw-r--r--   0     1001      127     1020 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/new_syntax/new_lookup.slint
+-rw-r--r--   0     1001      127     8651 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/new_syntax/two_way_input_output.slint
+-rw-r--r--   0     1001      127      252 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/parse_error/children_placeholder0.slint
+-rw-r--r--   0     1001      127      263 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/parse_error/export0.slint
+-rw-r--r--   0     1001      127      219 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/parse_error/export1.slint
+-rw-r--r--   0     1001      127      362 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/parse_error/if0.slint
+-rw-r--r--   0     1001      127      278 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/parse_error/if1.slint
+-rw-r--r--   0     1001      127      285 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/parse_error/if2.slint
+-rw-r--r--   0     1001      127      224 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/parse_error/if3.slint
+-rw-r--r--   0     1001      127      361 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/parse_error/if4.slint
+-rw-r--r--   0     1001      127      398 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/parse_error/property1.slint
+-rw-r--r--   0     1001      127      902 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/parse_error/property2.slint
+-rw-r--r--   0     1001      127      846 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/parse_error/state1.slint
+-rw-r--r--   0     1001      127      244 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/parse_error/state2.slint
+-rw-r--r--   0     1001      127      307 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/parse_error/state3.slint
+-rw-r--r--   0     1001      127      707 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/parse_error/struct.slint
+-rw-r--r--   0     1001      127     9418 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax_tests.rs
+-rw-r--r--   0     1001      127      156 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/typeloader/custom_style/TestStyle/std-widgets.slint
+-rw-r--r--   0     1001      127      278 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/typeloader/dependency_local.slint
+-rw-r--r--   0     1001      127      393 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/typeloader/dependency_test_main.slint
+-rw-r--r--   0     1001      127      503 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/typeloader/incpath/bug_2719_import.slint
+-rw-r--r--   0     1001      127      461 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/typeloader/incpath/bug_3674_alias_from_invalid_import.slint
+-rw-r--r--   0     1001      127      262 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/typeloader/incpath/dependency_from_incpath.slint
+-rw-r--r--   0     1001      127      205 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/typeloader/incpath/local_helper_type.slint
+-rw-r--r--   0     1001      127      237 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/typeloader/incpath/should_fail.slint
+-rw-r--r--   0     1001      127      320 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/typeloader/incpath/should_fail2.slint
+-rw-r--r--   0     1001      127      280 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/typeloader/incpath/should_fail3.slint
+-rw-r--r--   0     1001      127      491 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/typeloader/incpath/should_fail4.slint
+-rw-r--r--   0     1001      127      208 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/typeloader/library/dependency_from_library.slint
+-rw-r--r--   0     1001      127      243 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/typeloader/library/lib.slint
+-rw-r--r--   0     1001      127      214 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/typeloader/library/library_helper_type.slint
+-rw-r--r--   0     1001      127      324 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/typeloader/recursive_import1.slint
+-rw-r--r--   0     1001      127      395 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/typeloader/recursive_import2.slint
+-rw-r--r--   0     1001      127      450 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/typeloader/some_rust_file.rs
+-rw-r--r--   0     1001      127    43496 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/typeloader.rs
+-rw-r--r--   0     1001      127    19774 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/typeregister.rs
+-rw-r--r--   0     1001      127    14083 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/common/MadeWithSlint-logo-dark.svg
+-rw-r--r--   0     1001      127    14073 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/common/MadeWithSlint-logo-light.svg
+-rw-r--r--   0     1001      127     2358 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/common/combobox-base.slint
+-rw-r--r--   0     1001      127     3861 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/common/common.slint
+-rw-r--r--   0     1001      127     3266 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/common/lineedit-base.slint
+-rw-r--r--   0     1001      127     4288 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/common/listview.slint
+-rw-r--r--   0     1001      127     3926 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/common/slider-base.slint
+-rw-r--r--   0     1001      127     2427 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/common/spinbox-base.slint
+-rw-r--r--   0     1001      127     2510 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/common/spinner-base.slint
+-rw-r--r--   0     1001      127     1202 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/common/standardbutton.slint
+-rw-r--r--   0     1001      127     1080 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/common/tabwidget-base.slint
+-rw-r--r--   0     1001      127      268 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic/color-scheme.slint
+-rw-r--r--   0     1001      127      329 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic/std-widgets-impl.slint
+-rw-r--r--   0     1001      127      212 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic/std-widgets.slint
+-rw-r--r--   0     1001      127      308 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-base/_arrow_down.svg
+-rw-r--r--   0     1001      127      284 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-base/_arrow_up.svg
+-rw-r--r--   0     1001      127      413 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-base/_check-mark.svg
+-rw-r--r--   0     1001      127      148 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-base/_pane_down.svg
+-rw-r--r--   0     1001      127     2760 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-base/button.slint
+-rw-r--r--   0     1001      127     2726 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-base/checkbox.slint
+-rw-r--r--   0     1001      127     3057 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-base/combobox.slint
+-rw-r--r--   0     1001      127     4437 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-base/components.slint
+-rw-r--r--   0     1001      127     1000 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-base/groupbox.slint
+-rw-r--r--   0     1001      127      632 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-base/layouts.slint
+-rw-r--r--   0     1001      127     2886 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-base/lineedit.slint
+-rw-r--r--   0     1001      127      988 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-base/progressindicator.slint
+-rw-r--r--   0     1001      127     5065 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-base/scrollview.slint
+-rw-r--r--   0     1001      127     2930 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-base/slider.slint
+-rw-r--r--   0     1001      127     3327 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-base/spinbox.slint
+-rw-r--r--   0     1001      127      733 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-base/spinner.slint
+-rw-r--r--   0     1001      127     1524 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-base/std-widgets-base.slint
+-rw-r--r--   0     1001      127     2126 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-base/std-widgets-impl.slint
+-rw-r--r--   0     1001      127     3420 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-base/styling.slint
+-rw-r--r--   0     1001      127     2861 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-base/switch.slint
+-rw-r--r--   0     1001      127     9124 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-base/tableview.slint
+-rw-r--r--   0     1001      127     6075 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-base/tabwidget.slint
+-rw-r--r--   0     1001      127     4438 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-base/textedit.slint
+-rw-r--r--   0     1001      127      257 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-dark/color-scheme.slint
+-rw-r--r--   0     1001      127      329 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-dark/std-widgets-impl.slint
+-rw-r--r--   0     1001      127      212 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-dark/std-widgets.slint
+-rw-r--r--   0     1001      127      258 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-light/color-scheme.slint
+-rw-r--r--   0     1001      127      329 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-light/std-widgets-impl.slint
+-rw-r--r--   0     1001      127      212 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-light/std-widgets.slint
+-rw-r--r--   0     1001      127      268 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino/color-scheme.slint
+-rw-r--r--   0     1001      127      332 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino/std-widgets-impl.slint
+-rw-r--r--   0     1001      127      215 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino/std-widgets.slint
+-rw-r--r--   0     1001      127      513 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/_arrow-down.svg
+-rw-r--r--   0     1001      127      507 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/_arrow-up.svg
+-rw-r--r--   0     1001      127      780 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/_check-mark.svg
+-rw-r--r--   0     1001      127      623 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/_chevron-down.svg
+-rw-r--r--   0     1001      127      601 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/_chevron-up.svg
+-rw-r--r--   0     1001      127      918 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/_down.svg
+-rw-r--r--   0     1001      127      489 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/_dropdown.svg
+-rw-r--r--   0     1001      127      849 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/_left.svg
+-rw-r--r--   0     1001      127      815 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/_right.svg
+-rw-r--r--   0     1001      127     1135 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/_up.svg
+-rw-r--r--   0     1001      127     5181 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/button.slint
+-rw-r--r--   0     1001      127     4547 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/checkbox.slint
+-rw-r--r--   0     1001      127     5646 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/combobox.slint
+-rw-r--r--   0     1001      127     3145 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/components.slint
+-rw-r--r--   0     1001      127     1103 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/groupbox.slint
+-rw-r--r--   0     1001      127      632 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/layouts.slint
+-rw-r--r--   0     1001      127     3180 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/lineedit.slint
+-rw-r--r--   0     1001      127     1404 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/progressindicator.slint
+-rw-r--r--   0     1001      127     5563 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/scrollview.slint
+-rw-r--r--   0     1001      127     3097 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/slider.slint
+-rw-r--r--   0     1001      127     5483 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/spinbox.slint
+-rw-r--r--   0     1001      127      739 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/spinner.slint
+-rw-r--r--   0     1001      127     1524 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/std-widgets-base.slint
+-rw-r--r--   0     1001      127     2216 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/std-widgets-impl.slint
+-rw-r--r--   0     1001      127     4541 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/styling.slint
+-rw-r--r--   0     1001      127     4097 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/switch.slint
+-rw-r--r--   0     1001      127     8959 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/tableview.slint
+-rw-r--r--   0     1001      127     5493 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/tabwidget.slint
+-rw-r--r--   0     1001      127     6640 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/textedit.slint
+-rw-r--r--   0     1001      127      257 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-dark/color-scheme.slint
+-rw-r--r--   0     1001      127      332 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-dark/std-widgets-impl.slint
+-rw-r--r--   0     1001      127      215 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-dark/std-widgets.slint
+-rw-r--r--   0     1001      127      258 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-light/color-scheme.slint
+-rw-r--r--   0     1001      127      332 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-light/std-widgets-impl.slint
+-rw-r--r--   0     1001      127      215 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-light/std-widgets.slint
+-rw-r--r--   0     1001      127      268 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent/color-scheme.slint
+-rw-r--r--   0     1001      127      329 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent/std-widgets-impl.slint
+-rw-r--r--   0     1001      127      212 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent/std-widgets.slint
+-rw-r--r--   0     1001      127      513 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/_arrow-down.svg
+-rw-r--r--   0     1001      127      507 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/_arrow-up.svg
+-rw-r--r--   0     1001      127      780 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/_check-mark.svg
+-rw-r--r--   0     1001      127      623 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/_chevron-down.svg
+-rw-r--r--   0     1001      127      601 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/_chevron-up.svg
+-rw-r--r--   0     1001      127      918 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/_down.svg
+-rw-r--r--   0     1001      127      489 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/_dropdown.svg
+-rw-r--r--   0     1001      127      849 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/_left.svg
+-rw-r--r--   0     1001      127      815 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/_right.svg
+-rw-r--r--   0     1001      127     1135 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/_up.svg
+-rw-r--r--   0     1001      127     4607 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/button.slint
+-rw-r--r--   0     1001      127     3883 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/checkbox.slint
+-rw-r--r--   0     1001      127     3773 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/combobox.slint
+-rw-r--r--   0     1001      127     3363 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/components.slint
+-rw-r--r--   0     1001      127      877 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/groupbox.slint
+-rw-r--r--   0     1001      127      632 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/layouts.slint
+-rw-r--r--   0     1001      127     3499 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/lineedit.slint
+-rw-r--r--   0     1001      127     1023 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/progressindicator.slint
+-rw-r--r--   0     1001      127     6590 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/scrollview.slint
+-rw-r--r--   0     1001      127     3734 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/slider.slint
+-rw-r--r--   0     1001      127     3992 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/spinbox.slint
+-rw-r--r--   0     1001      127      733 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/spinner.slint
+-rw-r--r--   0     1001      127     1524 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/std-widgets-base.slint
+-rw-r--r--   0     1001      127     2126 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/std-widgets-impl.slint
+-rw-r--r--   0     1001      127     6248 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/styling.slint
+-rw-r--r--   0     1001      127     4616 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/switch.slint
+-rw-r--r--   0     1001      127     9561 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/tableview.slint
+-rw-r--r--   0     1001      127     5493 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/tabwidget.slint
+-rw-r--r--   0     1001      127     4935 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/textedit.slint
+-rw-r--r--   0     1001      127      257 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-dark/color-scheme.slint
+-rw-r--r--   0     1001      127      329 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-dark/std-widgets-impl.slint
+-rw-r--r--   0     1001      127      212 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-dark/std-widgets.slint
+-rw-r--r--   0     1001      127      258 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-light/color-scheme.slint
+-rw-r--r--   0     1001      127      329 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-light/std-widgets-impl.slint
+-rw-r--r--   0     1001      127      212 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-light/std-widgets.slint
+-rw-r--r--   0     1001      127      268 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material/color-scheme.slint
+-rw-r--r--   0     1001      127      347 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material/std-widgets-impl.slint
+-rw-r--r--   0     1001      127      214 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material/std-widgets.slint
+-rw-r--r--   0     1001      127      163 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-base/_arrow-downward.svg
+-rw-r--r--   0     1001      127      115 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-base/_arrow-drop-down.svg
+-rw-r--r--   0     1001      127      115 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-base/_arrow-drop-up.svg
+-rw-r--r--   0     1001      127      161 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-base/_arrow-upward.svg
+-rw-r--r--   0     1001      127      150 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-base/_check-mark.svg
+-rw-r--r--   0     1001      127      145 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-base/_expand-more.svg
+-rw-r--r--   0     1001      127     3288 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-base/button.slint
+-rw-r--r--   0     1001      127     5664 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-base/checkbox.slint
+-rw-r--r--   0     1001      127     3452 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-base/combobox.slint
+-rw-r--r--   0     1001      127     4712 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-base/components.slint
+-rw-r--r--   0     1001      127     1477 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-base/groupbox.slint
+-rw-r--r--   0     1001      127      633 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-base/layouts.slint
+-rw-r--r--   0     1001      127     2866 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-base/lineedit.slint
+-rw-r--r--   0     1001      127     1010 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-base/progressindicator.slint
+-rw-r--r--   0     1001      127     5014 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-base/scrollview.slint
+-rw-r--r--   0     1001      127     4146 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-base/slider.slint
+-rw-r--r--   0     1001      127     5090 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-base/spinbox.slint
+-rw-r--r--   0     1001      127      737 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-base/spinner.slint
+-rw-r--r--   0     1001      127     1373 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-base/std-widgets-base.slint
+-rw-r--r--   0     1001      127     2213 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-base/std-widgets-impl.slint
+-rw-r--r--   0     1001      127     3651 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-base/styling.slint
+-rw-r--r--   0     1001      127     6174 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-base/switch.slint
+-rw-r--r--   0     1001      127     8186 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-base/tableview.slint
+-rw-r--r--   0     1001      127     4886 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-base/tabwidget.slint
+-rw-r--r--   0     1001      127      257 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-dark/color-scheme.slint
+-rw-r--r--   0     1001      127      331 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-dark/std-widgets-impl.slint
+-rw-r--r--   0     1001      127      214 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-dark/std-widgets.slint
+-rw-r--r--   0     1001      127      258 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-light/color-scheme.slint
+-rw-r--r--   0     1001      127      331 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-light/std-widgets-impl.slint
+-rw-r--r--   0     1001      127      214 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-light/std-widgets.slint
+-rw-r--r--   0     1001      127     1736 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/qt/button.slint
+-rw-r--r--   0     1001      127      350 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/qt/checkbox.slint
+-rw-r--r--   0     1001      127     1707 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/qt/combobox.slint
+-rw-r--r--   0     1001      127      582 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/qt/groupbox.slint
+-rw-r--r--   0     1001      127     2384 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/qt/internal-scrollview.slint
+-rw-r--r--   0     1001      127      613 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/qt/layouts.slint
+-rw-r--r--   0     1001      127     2377 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/qt/lineedit.slint
+-rw-r--r--   0     1001      127      307 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/qt/progressindicator.slint
+-rw-r--r--   0     1001      127     1026 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/qt/scrollview.slint
+-rw-r--r--   0     1001      127      447 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/qt/slider.slint
+-rw-r--r--   0     1001      127      859 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/qt/spinbox.slint
+-rw-r--r--   0     1001      127     1265 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/qt/spinner.slint
+-rw-r--r--   0     1001      127      374 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/qt/std-widgets-impl.slint
+-rw-r--r--   0     1001      127     1475 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/qt/std-widgets.slint
+-rw-r--r--   0     1001      127      346 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/qt/switch.slint
+-rw-r--r--   0     1001      127     5310 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/qt/tableview.slint
+-rw-r--r--   0     1001      127     1564 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/qt/tabwidget.slint
+-rw-r--r--   0     1001      127     1126 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/common/Cargo.toml
+-rw-r--r--   0     1001      127    34670 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/common/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0     1001      127     8815 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/common/LICENSES/LicenseRef-DejaVu-Font.txt
+-rw-r--r--   0     1001      127     3475 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/common/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
+-rw-r--r--   0     1001      127    14063 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/common/LICENSES/LicenseRef-Slint-commercial.md
+-rw-r--r--   0     1001      127      635 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/common/README.md
+-rw-r--r--   0     1001      127     7636 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/common/builtin_structs.rs
+-rw-r--r--   0     1001      127    19656 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/common/enums.rs
+-rw-r--r--   0     1001      127     8311 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/common/key_codes.rs
+-rw-r--r--   0     1001      127     1322 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/common/lib.rs
+-rw-r--r--   0     1001      127   757076 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/common/sharedfontdb/DejaVuSans.ttf
+-rw-r--r--   0     1001      127      145 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/common/sharedfontdb/DejaVuSans.ttf.license
+-rw-r--r--   0     1001      127     4526 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/common/sharedfontdb/fontconfig.rs
+-rw-r--r--   0     1001      127     7491 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/common/sharedfontdb.rs
+-rw-r--r--   0     1001      127      630 2024-05-03 06:06:50.000000 slint-1.6.0a7/helper_crates/const-field-offset/Cargo.toml
+-rw-r--r--   0     1001      127      610 2024-05-03 06:06:50.000000 slint-1.6.0a7/helper_crates/const-field-offset/CHANGELOG.md
+-rw-r--r--   0     1001      127    10280 2024-05-03 06:06:50.000000 slint-1.6.0a7/helper_crates/const-field-offset/LICENSES/Apache-2.0.txt
+-rw-r--r--   0     1001      127     1078 2024-05-03 06:06:50.000000 slint-1.6.0a7/helper_crates/const-field-offset/LICENSES/MIT.txt
+-rw-r--r--   0     1001      127      492 2024-05-03 06:06:50.000000 slint-1.6.0a7/helper_crates/const-field-offset/README.md
+-rw-r--r--   0     1001      127     6982 2024-05-03 06:06:50.000000 slint-1.6.0a7/helper_crates/const-field-offset/src/lib.rs
+-rw-r--r--   0     1001      127     4766 2024-05-03 06:06:50.000000 slint-1.6.0a7/helper_crates/const-field-offset/tests/test_field_offset.rs
+-rw-r--r--   0     1001      127      826 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/testing/Cargo.toml
+-rw-r--r--   0     1001      127     4705 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/testing/README.md
+-rw-r--r--   0     1001      127      845 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/testing/ffi.rs
+-rw-r--r--   0     1001      127     2990 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/testing/internal_tests.rs
+-rw-r--r--   0     1001      127     1695 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/testing/lib.rs
+-rw-r--r--   0     1001      127     5754 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/testing/search_api.rs
+-rw-r--r--   0     1001      127     6991 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/testing/testing_backend.rs
+-rw-r--r--   0     1001      127      571 2024-05-03 06:06:50.000000 slint-1.6.0a7/helper_crates/vtable/macro/Cargo.toml
+-rw-r--r--   0     1001      127    10280 2024-05-03 06:06:50.000000 slint-1.6.0a7/helper_crates/vtable/macro/LICENSES/Apache-2.0.txt
+-rw-r--r--   0     1001      127     1078 2024-05-03 06:06:50.000000 slint-1.6.0a7/helper_crates/vtable/macro/LICENSES/MIT.txt
+-rw-r--r--   0     1001      127    31632 2024-05-03 06:06:50.000000 slint-1.6.0a7/helper_crates/vtable/macro/macro.rs
+-rw-r--r--   0     1001      127     1919 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/renderers/femtovg/Cargo.toml
+-rw-r--r--   0     1001      127    34670 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/renderers/femtovg/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0     1001      127     3475 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/renderers/femtovg/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
+-rw-r--r--   0     1001      127    14063 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/renderers/femtovg/LICENSES/LicenseRef-Slint-commercial.md
+-rw-r--r--   0     1001      127      507 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/renderers/femtovg/README.md
+-rw-r--r--   0     1001      127    26501 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/renderers/femtovg/fonts.rs
+-rw-r--r--   0     1001      127     9732 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/renderers/femtovg/images.rs
+-rw-r--r--   0     1001      127    61993 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/renderers/femtovg/itemrenderer.rs
+-rw-r--r--   0     1001      127    23205 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/renderers/femtovg/lib.rs
+-rw-r--r--   0     1001      127     2370 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/selector/Cargo.toml
+-rw-r--r--   0     1001      127    34670 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/selector/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0     1001      127     3475 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/selector/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
+-rw-r--r--   0     1001      127    14063 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/selector/LICENSES/LicenseRef-Slint-commercial.md
+-rw-r--r--   0     1001      127      872 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/selector/README.md
+-rw-r--r--   0     1001      127     2014 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/selector/build.rs
+-rw-r--r--   0     1001      127     5859 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/selector/lib.rs
+-rw-r--r--   0     1001      127      623 2024-05-03 06:06:50.000000 slint-1.6.0a7/helper_crates/vtable/Cargo.toml
+-rw-r--r--   0     1001      127     1796 2024-05-03 06:06:50.000000 slint-1.6.0a7/helper_crates/vtable/CHANGELOG.md
+-rw-r--r--   0     1001      127    10280 2024-05-03 06:06:50.000000 slint-1.6.0a7/helper_crates/vtable/LICENSES/Apache-2.0.txt
+-rw-r--r--   0     1001      127     1078 2024-05-03 06:06:50.000000 slint-1.6.0a7/helper_crates/vtable/LICENSES/MIT.txt
+-rw-r--r--   0     1001      127      399 2024-05-03 06:06:50.000000 slint-1.6.0a7/helper_crates/vtable/README.md
+-rw-r--r--   0     1001      127     3723 2024-05-03 06:06:50.000000 slint-1.6.0a7/helper_crates/vtable/src/compile_fail_tests.rs
+-rw-r--r--   0     1001      127    18776 2024-05-03 06:06:50.000000 slint-1.6.0a7/helper_crates/vtable/src/lib.rs
+-rw-r--r--   0     1001      127    18973 2024-05-03 06:06:50.000000 slint-1.6.0a7/helper_crates/vtable/src/vrc.rs
+-rw-r--r--   0     1001      127     9552 2024-05-03 06:06:50.000000 slint-1.6.0a7/helper_crates/vtable/tests/test_vrc.rs
+-rw-r--r--   0     1001      127     5359 2024-05-03 06:06:50.000000 slint-1.6.0a7/helper_crates/vtable/tests/test_vtable.rs
+-rw-r--r--   0     1001      127      471 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/parser-test-macro/Cargo.toml
+-rw-r--r--   0     1001      127      887 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/parser-test-macro/README.md
+-rw-r--r--   0     1001      127     5619 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/parser-test-macro/lib.rs
+-rw-r--r--   0     1001      127     4483 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/Cargo.toml
+-rw-r--r--   0     1001      127    34670 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0     1001      127     3475 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
+-rw-r--r--   0     1001      127    14063 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/LICENSES/LicenseRef-Slint-commercial.md
+-rw-r--r--   0     1001      127      532 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/README.md
+-rw-r--r--   0     1001      127     2766 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/accessibility.rs
+-rw-r--r--   0     1001      127    13996 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/animations.rs
+-rw-r--r--   0     1001      127    38650 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/api.rs
+-rw-r--r--   0     1001      127     5210 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/callbacks.rs
+-rw-r--r--   0     1001      127     2586 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/component_factory.rs
+-rw-r--r--   0     1001      127     2926 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/context.rs
+-rw-r--r--   0     1001      127     7695 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/future.rs
+-rw-r--r--   0     1001      127     2503 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/graphics/bitmapfont.rs
+-rw-r--r--   0     1001      127    14664 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/graphics/border_radius.rs
+-rw-r--r--   0     1001      127     4038 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/graphics/boxshadowcache.rs
+-rw-r--r--   0     1001      127    14919 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/graphics/brush.rs
+-rw-r--r--   0     1001      127    17436 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/graphics/color.rs
+-rw-r--r--   0     1001      127     7064 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/graphics/image/cache.rs
+-rw-r--r--   0     1001      127     2528 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/graphics/image/htmlimage.rs
+-rw-r--r--   0     1001      127     3408 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/graphics/image/svg.rs
+-rw-r--r--   0     1001      127    48855 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/graphics/image.rs
+-rw-r--r--   0     1001      127    15911 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/graphics/path.rs
+-rw-r--r--   0     1001      127     6978 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/graphics/rendering_metrics_collector.rs
+-rw-r--r--   0     1001      127     8249 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/graphics.rs
+-rw-r--r--   0     1001      127    33891 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/input.rs
+-rw-r--r--   0     1001      127     8604 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/item_focus.rs
+-rw-r--r--   0     1001      127    32977 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/item_rendering.rs
+-rw-r--r--   0     1001      127    68108 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/item_tree.rs
+-rw-r--r--   0     1001      127     8608 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/items/component_container.rs
+-rw-r--r--   0     1001      127    17039 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/items/flickable.rs
+-rw-r--r--   0     1001      127     8722 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/items/image.rs
+-rw-r--r--   0     1001      127     5377 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/items/path.rs
+-rw-r--r--   0     1001      127    65922 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/items/text.rs
+-rw-r--r--   0     1001      127    46637 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/items.rs
+-rw-r--r--   0     1001      127    27945 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/layout.rs
+-rw-r--r--   0     1001      127     3347 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/lengths.rs
+-rw-r--r--   0     1001      127     2237 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/lib.rs
+-rw-r--r--   0     1001      127    47643 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/model/adapters.rs
+-rw-r--r--   0     1001      127     6658 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/model/model_peer.rs
+-rw-r--r--   0     1001      127    47304 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/model.rs
+-rw-r--r--   0     1001      127    16009 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/platform.rs
+-rw-r--r--   0     1001      127     7794 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/properties/change_tracker.rs
+-rw-r--r--   0     1001      127    18894 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/properties/ffi.rs
+-rw-r--r--   0     1001      127    38401 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/properties/properties_animations.rs
+-rw-r--r--   0     1001      127    59846 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/properties.rs
+-rw-r--r--   0     1001      127     5015 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/renderer.rs
+-rw-r--r--   0     1001      127    10886 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/rtti.rs
+-rw-r--r--   0     1001      127    21418 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/sharedvector.rs
+-rw-r--r--   0     1001      127     2865 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/slice.rs
+-rw-r--r--   0     1001      127    28862 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/software_renderer/draw_functions.rs
+-rw-r--r--   0     1001      127     3465 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/software_renderer/fixed.rs
+-rw-r--r--   0     1001      127     4673 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/software_renderer/fonts/pixelfont.rs
+-rw-r--r--   0     1001      127     3859 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/software_renderer/fonts/systemfonts.rs
+-rw-r--r--   0     1001      127     7334 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/software_renderer/fonts/vectorfont.rs
+-rw-r--r--   0     1001      127     5915 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/software_renderer/fonts.rs
+-rw-r--r--   0     1001      127   108310 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/software_renderer.rs
+-rw-r--r--   0     1001      127    13307 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/string.rs
+-rw-r--r--   0     1001      127     4182 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/tests.rs
+-rw-r--r--   0     1001      127    12929 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/textlayout/fragments.rs
+-rw-r--r--   0     1001      127     3222 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/textlayout/glyphclusters.rs
+-rw-r--r--   0     1001      127     1234 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/textlayout/linebreak_simple.rs
+-rw-r--r--   0     1001      127     1260 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/textlayout/linebreak_unicode.rs
+-rw-r--r--   0     1001      127    15364 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/textlayout/linebreaker.rs
+-rw-r--r--   0     1001      127    13512 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/textlayout/shaping.rs
+-rw-r--r--   0     1001      127    24952 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/textlayout.rs
+-rw-r--r--   0     1001      127    31757 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/timers.rs
+-rw-r--r--   0     1001      127     8992 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/translations.rs
+-rw-r--r--   0     1001      127     1884 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/unsafe_single_threaded.rs
+-rw-r--r--   0     1001      127    63165 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/window.rs
+-rw-r--r--   0     1001      127     3852 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/winit/Cargo.toml
+-rw-r--r--   0     1001      127    34670 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/winit/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0     1001      127     3475 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/winit/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
+-rw-r--r--   0     1001      127    14063 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/winit/LICENSES/LicenseRef-Slint-commercial.md
+-rw-r--r--   0     1001      127     2320 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/winit/README.md
+-rw-r--r--   0     1001      127    22398 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/winit/accesskit.rs
+-rw-r--r--   0     1001      127      474 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/winit/build.rs
+-rw-r--r--   0     1001      127    30209 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/winit/event_loop.rs
+-rw-r--r--   0     1001      127    16654 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/winit/lib.rs
+-rw-r--r--   0     1001      127     8046 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/winit/renderer/femtovg/glcontext.rs
+-rw-r--r--   0     1001      127     2131 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/winit/renderer/femtovg.rs
+-rw-r--r--   0     1001      127     4558 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/winit/renderer/skia.rs
+-rw-r--r--   0     1001      127     6824 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/winit/renderer/sw.rs
+-rw-r--r--   0     1001      127    14717 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/winit/wasm_input_helper.rs
+-rw-r--r--   0     1001      127    32085 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/winit/winitwindowadapter.rs
+-rw-r--r--   0     1001      127     2855 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/renderers/skia/Cargo.toml
+-rw-r--r--   0     1001      127    34670 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/renderers/skia/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0     1001      127     3475 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/renderers/skia/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
+-rw-r--r--   0     1001      127    14063 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/renderers/skia/LICENSES/LicenseRef-Slint-commercial.md
+-rw-r--r--   0     1001      127      507 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/renderers/skia/README.md
+-rw-r--r--   0     1001      127      673 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/renderers/skia/build.rs
+-rw-r--r--   0     1001      127     6875 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/renderers/skia/cached_image.rs
+-rw-r--r--   0     1001      127    14877 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/renderers/skia/d3d_surface.rs
+-rw-r--r--   0     1001      127    37207 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/renderers/skia/itemrenderer.rs
+-rw-r--r--   0     1001      127    23253 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/renderers/skia/lib.rs
+-rw-r--r--   0     1001      127     6372 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/renderers/skia/metal_surface.rs
+-rw-r--r--   0     1001      127    15370 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/renderers/skia/opengl_surface.rs
+-rw-r--r--   0     1001      127     4611 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/renderers/skia/software_surface.rs
+-rw-r--r--   0     1001      127    11843 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/renderers/skia/textlayout.rs
+-rw-r--r--   0     1001      127    17420 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/renderers/skia/vulkan_surface.rs
+-rw-r--r--   0     1001      127      706 2024-05-03 06:06:50.000000 slint-1.6.0a7/helper_crates/const-field-offset/macro/Cargo.toml
+-rw-r--r--   0     1001      127    12200 2024-05-03 06:06:50.000000 slint-1.6.0a7/helper_crates/const-field-offset/macro/macro.rs
+-rw-r--r--   0     1001      127     6405 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/interpreter/Cargo.toml
+-rw-r--r--   0     1001      127    34670 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/interpreter/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0     1001      127     3475 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/interpreter/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
+-rw-r--r--   0     1001      127    14063 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/interpreter/LICENSES/LicenseRef-Slint-commercial.md
+-rw-r--r--   0     1001      127    68256 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/interpreter/api.rs
+-rw-r--r--   0     1001      127    86334 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/interpreter/dynamic_item_tree.rs
+-rw-r--r--   0     1001      127     7555 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/interpreter/dynamic_type.rs
+-rw-r--r--   0     1001      127    75104 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/interpreter/eval.rs
+-rw-r--r--   0     1001      127    12240 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/interpreter/eval_layout.rs
+-rw-r--r--   0     1001      127    31460 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/interpreter/ffi.rs
+-rw-r--r--   0     1001      127     9875 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/interpreter/global_component.rs
+-rw-r--r--   0     1001      127     5912 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/interpreter/highlight.rs
+-rw-r--r--   0     1001      127     3029 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/interpreter/lib.rs
+-rw-r--r--   0     1001      127     1425 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/interpreter/migration.rs
+-rw-r--r--   0     1001      127     1809 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/interpreter/tests.rs
+-rw-r--r--   0     1001      127     2301 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/interpreter/value_model.rs
+-rw-r--r--   0     1001      127     9909 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/Cargo.toml
+-rw-r--r--   0     1001      127    34670 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0     1001      127     3475 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
+-rw-r--r--   0     1001      127    14063 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/LICENSES/LicenseRef-Slint-commercial.md
+-rw-r--r--   0     1001      127     1078 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/LICENSES/MIT.txt
+-rw-r--r--   0     1001      127     1881 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/README.md
+-rw-r--r--   0     1001      127     5140 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/android.rs
+-rw-r--r--   0     1001      127      548 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/compile_fail_tests.rs
+-rw-r--r--   0     1001      127     9447 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/building.md
+-rw-r--r--   0     1001      127     7147 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/development.md
+-rw-r--r--   0     1001      127     2881 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/install_qt.md
+-rw-r--r--   0     1001      127        5 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/.gitignore
+-rw-r--r--   0     1001      127     1013 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/README.md
+-rw-r--r--   0     1001      127      261 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/book.toml
+-rw-r--r--   0     1001      127      810 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/CMakeLists.txt
+-rw-r--r--   0     1001      127      515 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/SUMMARY.md
+-rw-r--r--   0     1001      127      268 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/appwindow.slint
+-rw-r--r--   0     1001      127     1216 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/conclusion.md
+-rw-r--r--   0     1001      127     1337 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/creating_the_tiles_from_cpp.md
+-rw-r--r--   0     1001      127     2039 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/from_one_to_multiple_tiles.md
+-rw-r--r--   0     1001      127     2483 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/game_logic_in_cpp.md
+-rw-r--r--   0     1001      127     2126 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/getting_started.md
+-rw-r--r--   0     1001      127      477 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/README.md
+-rw-r--r--   0     1001      127     1122 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/at-solid.svg
+-rw-r--r--   0     1001      127     3210 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/at.png
+-rw-r--r--   0     1001      127      971 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/balance-scale-solid.svg
+-rw-r--r--   0     1001      127     2265 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/balance-scale.png
+-rw-r--r--   0     1001      127     1577 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/bicycle-solid.svg
+-rw-r--r--   0     1001      127     2613 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/bicycle.png
+-rw-r--r--   0     1001      127      837 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/bus-solid.svg
+-rw-r--r--   0     1001      127     1540 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/bus.png
+-rw-r--r--   0     1001      127      485 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/cloud-solid.svg
+-rw-r--r--   0     1001      127     1454 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/cloud.png
+-rw-r--r--   0     1001      127     2614 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/cogs-solid.svg
+-rw-r--r--   0     1001      127     2894 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/cogs.png
+-rw-r--r--   0     1001      127     1252 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/motorcycle-solid.svg
+-rw-r--r--   0     1001      127     2497 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/motorcycle.png
+-rw-r--r--   0     1001      127     6059 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/tile_logo.png
+-rw-r--r--   0     1001      127      467 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/video-solid.svg
+-rw-r--r--   0     1001      127     1073 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/video.png
+-rw-r--r--   0     1001      127     1060 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/ideas_for_the_reader.md
+-rw-r--r--   0     1001      127      953 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/introduction.md
+-rw-r--r--   0     1001      127     2800 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/main_game_logic.cpp
+-rw-r--r--   0     1001      127      300 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/main_initial.cpp
+-rw-r--r--   0     1001      127      877 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/main_tiles_from_cpp.cpp
+-rw-r--r--   0     1001      127     2636 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/memory_game_logic.slint
+-rw-r--r--   0     1001      127     2130 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/memory_tile.md
+-rw-r--r--   0     1001      127      425 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/memory_tile.slint
+-rw-r--r--   0     1001      127     2221 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/memory_tiles_from_cpp.slint
+-rw-r--r--   0     1001      127     2760 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/polishing_the_tile.md
+-rw-r--r--   0     1001      127      262 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/book.toml
+-rw-r--r--   0     1001      127      527 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/SUMMARY.md
+-rw-r--r--   0     1001      127     1223 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/conclusion.md
+-rw-r--r--   0     1001      127     1191 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/creating_the_tiles_from_js.md
+-rw-r--r--   0     1001      127     2034 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/from_one_to_multiple_tiles.md
+-rw-r--r--   0     1001      127     2031 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/game_logic_in_js.md
+-rw-r--r--   0     1001      127     1515 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/getting_started.md
+-rw-r--r--   0     1001      127      477 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/README.md
+-rw-r--r--   0     1001      127     1122 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/at-solid.svg
+-rw-r--r--   0     1001      127     3210 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/at.png
+-rw-r--r--   0     1001      127      971 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/balance-scale-solid.svg
+-rw-r--r--   0     1001      127     2265 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/balance-scale.png
+-rw-r--r--   0     1001      127     1577 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/bicycle-solid.svg
+-rw-r--r--   0     1001      127     2613 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/bicycle.png
+-rw-r--r--   0     1001      127      837 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/bus-solid.svg
+-rw-r--r--   0     1001      127     1540 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/bus.png
+-rw-r--r--   0     1001      127      485 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/cloud-solid.svg
+-rw-r--r--   0     1001      127     1454 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/cloud.png
+-rw-r--r--   0     1001      127     2614 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/cogs-solid.svg
+-rw-r--r--   0     1001      127     2894 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/cogs.png
+-rw-r--r--   0     1001      127     1252 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/motorcycle-solid.svg
+-rw-r--r--   0     1001      127     2497 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/motorcycle.png
+-rw-r--r--   0     1001      127     6059 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/tile_logo.png
+-rw-r--r--   0     1001      127      467 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/video-solid.svg
+-rw-r--r--   0     1001      127     1073 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/video.png
+-rw-r--r--   0     1001      127     1060 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/ideas_for_the_reader.md
+-rw-r--r--   0     1001      127      960 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/introduction.md
+-rw-r--r--   0     1001      127     1797 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/main_game_logic.js
+-rw-r--r--   0     1001      127      275 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/main_initial.js
+-rw-r--r--   0     1001      127      631 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/main_tiles_from_js.js
+-rw-r--r--   0     1001      127      265 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/memory.slint
+-rw-r--r--   0     1001      127     2636 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/memory_game_logic.slint
+-rw-r--r--   0     1001      127     2079 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/memory_tile.md
+-rw-r--r--   0     1001      127      425 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/memory_tile.slint
+-rw-r--r--   0     1001      127     2221 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/memory_tiles_from_cpp.slint
+-rw-r--r--   0     1001      127      202 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/package.json
+-rw-r--r--   0     1001      127     2747 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/polishing_the_tile.md
+-rw-r--r--   0     1001      127      262 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/rust/book.toml
+-rw-r--r--   0     1001      127     3821 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/theme/head.hbs
+-rw-r--r--   0     1001      127       84 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/theme/highlight.css
+-rw-r--r--   0     1001      127      282 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/theme/highlight.js
+-rw-r--r--   0     1001      127      386 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/Pipfile
+-rw-r--r--   0     1001      127      256 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/_static/theme_tweak.css
+-rw-r--r--   0     1001      127      190 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/_templates/base.html
+-rw-r--r--   0     1001      127     4339 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/conf.py
+-rw-r--r--   0     1001      127      811 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/index.rst
+-rw-r--r--   0     1001      127     7746 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/advanced/backend_linuxkms.md
+-rw-r--r--   0     1001      127     1061 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/advanced/backend_qt.md
+-rw-r--r--   0     1001      127     1692 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/advanced/backend_winit.md
+-rw-r--r--   0     1001      127     7431 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/advanced/backends_and_renderers.md
+-rw-r--r--   0     1001      127     6034 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/advanced/debugging_techniques.md
+-rw-r--r--   0     1001      127     3816 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/advanced/style.md
+-rw-r--r--   0     1001      127     1095 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/introduction/index.md
+-rw-r--r--   0     1001      127     2287 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/introduction/supported_platforms.md
+-rw-r--r--   0     1001      127     1418 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/builtins/callbacks.md
+-rw-r--r--   0     1001      127    42035 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/builtins/elements.md
+-rw-r--r--   0     1001      127      975 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/builtins/functions.md
+-rw-r--r--   0     1001      127     3227 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/builtins/globals.md
+-rw-r--r--   0     1001      127      267 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/builtins/index.rst
+-rw-r--r--   0     1001      127     3567 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/builtins/namespaces.md
+-rw-r--r--   0     1001      127     1144 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/concepts/container.md
+-rw-r--r--   0     1001      127     2165 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/concepts/file.md
+-rw-r--r--   0     1001      127     2315 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/concepts/focus.md
+-rw-r--r--   0     1001      127     1232 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/concepts/fonts.md
+-rw-r--r--   0     1001      127      262 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/concepts/index.rst
+-rw-r--r--   0     1001      127    13939 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/concepts/layouting.md
+-rw-r--r--   0     1001      127     1787 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/concepts/purity.md
+-rw-r--r--   0     1001      127     7822 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/concepts/translations.md
+-rw-r--r--   0     1001      127     2235 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/index.rst
+-rw-r--r--   0     1001      127     2270 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/animations.md
+-rw-r--r--   0     1001      127     1627 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/callbacks.md
+-rw-r--r--   0     1001      127      326 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/comments.md
+-rw-r--r--   0     1001      127      492 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/conditions.md
+-rw-r--r--   0     1001      127     1792 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/expressions.md
+-rw-r--r--   0     1001      127     1821 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/functions.md
+-rw-r--r--   0     1001      127     2776 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/globals.md
+-rw-r--r--   0     1001      127      413 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/identifiers.md
+-rw-r--r--   0     1001      127      402 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/index.rst
+-rw-r--r--   0     1001      127      851 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/legacy_syntax.md
+-rw-r--r--   0     1001      127     3946 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/modules.md
+-rw-r--r--   0     1001      127     5168 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/properties.md
+-rw-r--r--   0     1001      127     1470 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/repetitions.md
+-rw-r--r--   0     1001      127      658 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/statements.md
+-rw-r--r--   0     1001      127     2210 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/states.md
+-rw-r--r--   0     1001      127    17651 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/types.md
+-rw-r--r--   0     1001      127      299 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/aboutslint.md
+-rw-r--r--   0     1001      127     1469 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/button.md
+-rw-r--r--   0     1001      127     1035 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/checkbox.md
+-rw-r--r--   0     1001      127     1087 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/combobox.md
+-rw-r--r--   0     1001      127      251 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/gridbox.md
+-rw-r--r--   0     1001      127      741 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/groupbox.md
+-rw-r--r--   0     1001      127      337 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/horizontalbox.md
+-rw-r--r--   0     1001      127      569 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/index.rst
+-rw-r--r--   0     1001      127     2460 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/lineedit.md
+-rw-r--r--   0     1001      127     1293 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/listview.md
+-rw-r--r--   0     1001      127      801 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/progressindicator.md
+-rw-r--r--   0     1001      127     1976 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/scrollview.md
+-rw-r--r--   0     1001      127     1145 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/slider.md
+-rw-r--r--   0     1001      127      866 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/spinbox.md
+-rw-r--r--   0     1001      127      805 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/spinner.md
+-rw-r--r--   0     1001      127     1071 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/standardbutton.md
+-rw-r--r--   0     1001      127     1489 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/standardlistview.md
+-rw-r--r--   0     1001      127     2176 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/standardtableview.md
+-rw-r--r--   0     1001      127     1037 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/switch.md
+-rw-r--r--   0     1001      127      800 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/tabwidget.md
+-rw-r--r--   0     1001      127     2301 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/textedit.md
+-rw-r--r--   0     1001      127      335 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/verticalbox.md
+-rw-r--r--   0     1001      127      565 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/widgets.md
+-rw-r--r--   0     1001      127      364 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/recipes/button_native.slint
+-rw-r--r--   0     1001      127    28191 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/recipes/recipes.md
+-rw-r--r--   0     1001      127     3821 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/resources/slint-docs-highlight.html
+-rw-r--r--   0     1001      127     5521 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/resources/slint-docs-preview.html
+-rw-r--r--   0     1001      127    14477 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/site/index.html
+-rw-r--r--   0     1001      127     3880 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/testing.md
+-rw-r--r--   0     1001      127     1698 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/torizon.md
+-rw-r--r--   0     1001      127     3775 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/triage.md
+-rw-r--r--   0     1001      127     6705 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs.rs
+-rw-r--r--   0     1001      127    14341 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/lib.rs
+-rw-r--r--   0     1001      127    20004 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/mcu.md
+-rw-r--r--   0     1001      127     7565 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/private_unstable_api.rs
+-rw-r--r--   0     1001      127     8976 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/tests/partial_renderer.rs
+-rw-r--r--   0     1001      127      890 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/tests/show_strongref.rs
+-rw-r--r--   0     1001      127     1147 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/tests/simple_macro.rs
+-rw-r--r--   0     1001      127     2491 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/tests/spawn_local.rs
+-rw-r--r--   0     1001      127     2557 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/type-mappings.md
+-rw-r--r--   0     1001      127     1109 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/android-activity/Cargo.toml
+-rw-r--r--   0     1001      127    34670 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/android-activity/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0     1001      127     3475 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/android-activity/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
+-rw-r--r--   0     1001      127    14063 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/android-activity/LICENSES/LicenseRef-Slint-commercial.md
+-rw-r--r--   0     1001      127      740 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/android-activity/README.md
+-rw-r--r--   0     1001      127    34583 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/android-activity/androidwindowadapter.rs
+-rw-r--r--   0     1001      127     4464 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/android-activity/build.rs
+-rw-r--r--   0     1001      127    18055 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/android-activity/java/SlintAndroidJavaHelper.java
+-rw-r--r--   0     1001      127    18156 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/android-activity/javahelper.rs
+-rw-r--r--   0     1001      127     6133 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/android-activity/lib.rs
+-rw-r--r--   0     1001      127      768 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/build/Cargo.toml
+-rw-r--r--   0     1001      127    34670 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/build/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0     1001      127     3475 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/build/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
+-rw-r--r--   0     1001      127    14063 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/build/LICENSES/LicenseRef-Slint-commercial.md
+-rw-r--r--   0     1001      127    15366 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/build/lib.rs
+-rw-r--r--   0     1001      127     1383 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/Cargo.toml
+-rw-r--r--   0     1001      127    34670 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0     1001      127     3475 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
+-rw-r--r--   0     1001      127    14063 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/LICENSES/LicenseRef-Slint-commercial.md
+-rw-r--r--   0     1001      127      507 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/README.md
+-rw-r--r--   0     1001      127    10783 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/accessible_generated.rs
+-rw-r--r--   0     1001      127     2995 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/build.rs
+-rw-r--r--   0     1001      127    27433 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/key_generated.rs
+-rw-r--r--   0     1001      127    10534 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/lib.rs
+-rw-r--r--   0     1001      127    32981 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/qt_accessible.rs
+-rw-r--r--   0     1001      127    21040 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/qt_widgets/button.rs
+-rw-r--r--   0     1001      127     6862 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/qt_widgets/checkbox.rs
+-rw-r--r--   0     1001      127     9594 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/qt_widgets/combobox.rs
+-rw-r--r--   0     1001      127     8992 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/qt_widgets/groupbox.rs
+-rw-r--r--   0     1001      127     5930 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/qt_widgets/lineedit.rs
+-rw-r--r--   0     1001      127     8178 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/qt_widgets/listviewitem.rs
+-rw-r--r--   0     1001      127     7422 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/qt_widgets/palette.rs
+-rw-r--r--   0     1001      127     4945 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/qt_widgets/progress_indicator.rs
+-rw-r--r--   0     1001      127    19794 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/qt_widgets/scrollview.rs
+-rw-r--r--   0     1001      127    13940 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/qt_widgets/slider.rs
+-rw-r--r--   0     1001      127    12535 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/qt_widgets/spinbox.rs
+-rw-r--r--   0     1001      127     8594 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/qt_widgets/stylemetrics.rs
+-rw-r--r--   0     1001      127     5637 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/qt_widgets/tableheadersection.rs
+-rw-r--r--   0     1001      127    22417 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/qt_widgets/tabwidget.rs
+-rw-r--r--   0     1001      127    12967 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/qt_widgets.rs
+-rw-r--r--   0     1001      127   107271 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/qt_window.rs
+-rw-r--r--   0     1001      127      532 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core-macros/Cargo.toml
+-rw-r--r--   0     1001      127    34670 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core-macros/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0     1001      127     3475 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core-macros/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
+-rw-r--r--   0     1001      127    14063 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core-macros/LICENSES/LicenseRef-Slint-commercial.md
+-rw-r--r--   0     1001      127      590 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core-macros/README.md
+-rw-r--r--   0     1001      127     7310 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core-macros/lib.rs
+-rw-r--r--   0        0        0      931 1970-01-01 00:00:00.000000 slint-1.6.0a7/api/python/Cargo.toml
+-rw-r--r--   0     1001      127       11 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/python/.gitignore
+-rw-r--r--   0     1001      127     7730 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/python/README.md
+-rw-r--r--   0     1001      127     4367 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/python/brush.rs
+-rw-r--r--   0     1001      127     3303 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/python/errors.rs
+-rw-r--r--   0     1001      127     1399 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/python/image.rs
+-rw-r--r--   0     1001      127    10939 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/python/interpreter.rs
+-rw-r--r--   0     1001      127     1421 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/python/lib.rs
+-rw-r--r--   0     1001      127     6300 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/python/models.rs
+-rw-r--r--   0     1001      127      348 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/python/noxfile.py
+-rw-r--r--   0     1001      127     7729 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/python/slint/__init__.py
+-rw-r--r--   0     1001      127     1889 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/python/slint/models.py
+-rw-r--r--   0     1001      127     1164 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/python/tests/test_brush.py
+-rw-r--r--   0     1001      127     1019 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/python/tests/test_callback_decorators.py
+-rw-r--r--   0     1001      127     2369 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/python/tests/test_compiler.py
+-rw-r--r--   0     1001      127     1095 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/python/tests/test_gc.py
+-rw-r--r--   0     1001      127     6577 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/python/tests/test_instance.py
+-rw-r--r--   0     1001      127     1597 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/python/tests/test_load_file.py
+-rw-r--r--   0     1001      127      905 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/python/tests/test_load_file.slint
+-rw-r--r--   0     1001      127      687 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/python/tests/test_loader.py
+-rw-r--r--   0     1001      127     3589 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/python/tests/test_models.py
+-rw-r--r--   0     1001      127      832 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/python/tests/test_timers.py
+-rw-r--r--   0     1001      127     2415 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/python/timer.rs
+-rw-r--r--   0     1001      127     4717 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/python/value.rs
+-rw-r--r--   0     1001      127   207946 2024-05-03 06:06:59.000000 slint-1.6.0a7/Cargo.lock
+-rw-r--r--   0        0        0     4140 1970-01-01 00:00:00.000000 slint-1.6.0a7/Cargo.toml
+-rw-r--r--   0        0        0     1487 1970-01-01 00:00:00.000000 slint-1.6.0a7/pyproject.toml
+-rw-r--r--   0     1001      127     7729 2024-05-03 06:06:50.000000 slint-1.6.0a7/slint/__init__.py
+-rw-r--r--   0     1001      127     1889 2024-05-03 06:06:50.000000 slint-1.6.0a7/slint/models.py
+-rw-r--r--   0        0        0     9277 1970-01-01 00:00:00.000000 slint-1.6.0a7/PKG-INFO
```

### Comparing `slint-1.6.0a6/internal/backends/winit/Cargo.toml` & `slint-1.6.0a7/internal/backends/winit/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/winit/LICENSES/GPL-3.0-only.txt` & `slint-1.6.0a7/api/rs/macros/LICENSES/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/winit/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md` & `slint-1.6.0a7/api/rs/macros/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/winit/LICENSES/LicenseRef-Slint-commercial.md` & `slint-1.6.0a7/api/rs/macros/LICENSES/LicenseRef-Slint-commercial.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/winit/README.md` & `slint-1.6.0a7/internal/backends/winit/README.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/winit/accesskit.rs` & `slint-1.6.0a7/internal/backends/winit/accesskit.rs`

 * *Files 3% similar despite different names*

```diff
@@ -122,15 +122,15 @@
 
     fn handle_request(&self, request: ActionRequest) {
         let Some(window_adapter) = self.window_adapter_weak.upgrade() else { return };
         let a = match request.action {
             Action::Default => AccessibilityAction::Default,
             Action::Focus => {
                 if let Some(item) = self.item_rc_for_node_id(request.target) {
-                    WindowInner::from_pub(window_adapter.window()).set_focus_item(&item);
+                    WindowInner::from_pub(window_adapter.window()).set_focus_item(&item, true);
                 }
                 return;
             }
             Action::Decrement => AccessibilityAction::Decrement,
             Action::Increment => AccessibilityAction::Increment,
             Action::ReplaceSelectedText => {
                 let Some(accesskit::ActionData::Value(v)) = request.data else { return };
@@ -370,19 +370,20 @@
             update = wait_condition.wait(update).unwrap();
         }
 
         update.take().unwrap()
     }
 
     fn build_node_without_children(&self, item: &ItemRc, scale_factor: ScaleFactor) -> NodeBuilder {
-        let is_checkable =
-            item.accessible_string_property(AccessibleStringProperty::Checkable) == "true";
+        let is_checkable = item
+            .accessible_string_property(AccessibleStringProperty::Checkable)
+            .is_some_and(|x| x == "true");
 
         let (role, label) = if let Some(window_item) = item.downcast::<WindowItem>() {
-            (Role::Window, window_item.as_pin_ref().title().to_string())
+            (Role::Window, Some(window_item.as_pin_ref().title().to_string()))
         } else {
             (
                 match item.accessible_role() {
                     i_slint_core::items::AccessibleRole::None => Role::Unknown,
                     i_slint_core::items::AccessibleRole::Button if is_checkable => {
                         Role::ToggleButton
                     }
@@ -402,73 +403,89 @@
                         Role::ProgressIndicator
                     }
                     i_slint_core::items::AccessibleRole::Switch => Role::Switch,
                 },
                 item.accessible_string_property(
                     i_slint_core::accessibility::AccessibleStringProperty::Label,
                 )
-                .to_string(),
+                .map(|x| x.to_string()),
             )
         };
 
         let mut builder = NodeBuilder::new(role);
 
-        builder.set_name(label);
+        if let Some(label) = label {
+            builder.set_name(label);
+        }
 
         let geometry = item.geometry();
         let absolute_origin = item.map_to_window(geometry.origin);
         let physical_origin = (absolute_origin * scale_factor).cast::<f64>();
         let physical_size = (geometry.size * scale_factor).cast::<f64>();
         builder.set_bounds(accesskit::Rect {
             x0: physical_origin.x,
             y0: physical_origin.y,
             x1: physical_origin.x + physical_size.width,
             y1: physical_origin.y + physical_size.height,
         });
 
         if is_checkable {
             builder.set_checked(
-                if item.accessible_string_property(AccessibleStringProperty::Checked) == "true" {
+                if item
+                    .accessible_string_property(AccessibleStringProperty::Checked)
+                    .is_some_and(|x| x == "true")
+                {
                     Checked::True
                 } else {
                     Checked::False
                 },
             );
         }
 
-        builder.set_description(
-            item.accessible_string_property(AccessibleStringProperty::Description).to_string(),
-        );
+        if let Some(description) =
+            item.accessible_string_property(AccessibleStringProperty::Description)
+        {
+            builder.set_description(description.to_string());
+        }
 
         if matches!(
             role,
             Role::Button
                 | Role::CheckBox
                 | Role::ComboBox
                 | Role::Slider
                 | Role::SpinButton
                 | Role::Tab
         ) {
             builder.add_action(Action::Focus);
         }
 
-        let min = item.accessible_string_property(AccessibleStringProperty::ValueMinimum);
-        let max = item.accessible_string_property(AccessibleStringProperty::ValueMaximum);
-        let step = item.accessible_string_property(AccessibleStringProperty::ValueStep);
-        let value = item.accessible_string_property(AccessibleStringProperty::Value).to_string();
-
-        match (min.parse(), max.parse(), value.parse(), step.parse()) {
-            (Ok(min), Ok(max), Ok(value), Ok(step)) => {
+        let min = item
+            .accessible_string_property(AccessibleStringProperty::ValueMinimum)
+            .unwrap_or_default();
+        let max = item
+            .accessible_string_property(AccessibleStringProperty::ValueMaximum)
+            .unwrap_or_default();
+        let step = item
+            .accessible_string_property(AccessibleStringProperty::ValueStep)
+            .unwrap_or_default();
+        match (min.parse(), max.parse(), step.parse()) {
+            (Ok(min), Ok(max), Ok(step)) => {
                 builder.set_min_numeric_value(min);
                 builder.set_max_numeric_value(max);
-                builder.set_numeric_value(value);
                 builder.set_numeric_value_step(step);
             }
-            _ => {
-                builder.set_value(value);
+            _ => {}
+        }
+
+        if let Some(value) = item.accessible_string_property(AccessibleStringProperty::Value) {
+            if let Ok(value) = value.parse() {
+                builder.set_numeric_value(value);
+            } else {
+                builder.set_value(value.to_string());
             }
         }
 
         let supported = item.supported_accessibility_actions();
         if supported.contains(SupportedAccessibilityAction::Default) {
             builder.add_action(accesskit::Action::Default)
         }
@@ -490,15 +507,15 @@
 }
 
 struct AccessibilitiesPropertyTracker {
     window_adapter_weak: Weak<WinitWindowAdapter>,
 }
 
 impl i_slint_core::properties::PropertyDirtyHandler for AccessibilitiesPropertyTracker {
-    fn notify(&self) {
+    fn notify(self: Pin<&Self>) {
         let win = self.window_adapter_weak.clone();
         i_slint_core::timers::Timer::single_shot(Default::default(), move || {
             if let Some(window_adapter) = win.upgrade() {
                 window_adapter.accesskit_adapter.rebuild_tree_of_dirty_nodes();
             };
         })
     }
```

### Comparing `slint-1.6.0a6/internal/backends/winit/event_loop.rs` & `slint-1.6.0a7/internal/backends/winit/event_loop.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/winit/lib.rs` & `slint-1.6.0a7/internal/backends/winit/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/winit/renderer/femtovg/glcontext.rs` & `slint-1.6.0a7/internal/backends/winit/renderer/femtovg/glcontext.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/winit/renderer/femtovg.rs` & `slint-1.6.0a7/internal/backends/winit/renderer/femtovg.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/winit/renderer/skia.rs` & `slint-1.6.0a7/internal/backends/winit/renderer/skia.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/winit/renderer/sw.rs` & `slint-1.6.0a7/internal/backends/winit/renderer/sw.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/winit/wasm_input_helper.rs` & `slint-1.6.0a7/internal/backends/winit/wasm_input_helper.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/winit/winitwindowadapter.rs` & `slint-1.6.0a7/internal/backends/winit/winitwindowadapter.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core/Cargo.toml` & `slint-1.6.0a7/internal/core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core/LICENSES/GPL-3.0-only.txt` & `slint-1.6.0a7/internal/backends/linuxkms/LICENSES/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md` & `slint-1.6.0a7/internal/backends/linuxkms/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core/LICENSES/LicenseRef-Slint-commercial.md` & `slint-1.6.0a7/internal/backends/linuxkms/LICENSES/LicenseRef-Slint-commercial.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core/README.md` & `slint-1.6.0a7/internal/core/README.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core/accessibility.rs` & `slint-1.6.0a7/internal/core/accessibility.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core/animations.rs` & `slint-1.6.0a7/internal/core/animations.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core/api.rs` & `slint-1.6.0a7/internal/core/api.rs`

 * *Files 0% similar despite different names*

```diff
@@ -615,15 +615,15 @@
 ///
 /// This trait is implemented by the compiler for each global singleton that's exported.
 ///
 /// # Example
 /// The following example of `.slint` markup defines a global singleton called `Palette`, exports
 /// it and modifies it from Rust code:
 /// ```rust
-/// # i_slint_backend_testing::init();
+/// # i_slint_backend_testing::init_no_event_loop();
 /// slint::slint!{
 /// export global Palette {
 ///     in property<color> foreground-color;
 ///     in property<color> background-color;
 /// }
 ///
 /// export component App inherits Window {
@@ -796,15 +796,15 @@
         /// On the next iteration of the event loop, the functor will be executed with a `T` as an argument.
         ///
         /// If the component was dropped because there are no more strong reference to the component,
         /// the functor will not be called.
         ///
         /// # Example
         /// ```rust
-        /// # i_slint_backend_testing::init();
+        /// # i_slint_backend_testing::init_no_event_loop();
         /// slint::slint! { export component MyApp inherits Window { in property <int> foo; /* ... */ } }
         /// let handle = MyApp::new().unwrap();
         /// let handle_weak = handle.as_weak();
         /// let thread = std::thread::spawn(move || {
         ///     // ... Do some computation in the thread
         ///     let foo = 42;
         ///     # assert!(handle_weak.upgrade().is_none()); // note that upgrade fails in a thread
@@ -852,15 +852,15 @@
 /// by collecting the code in a functor and queuing it up for invocation within the event loop.
 ///
 /// See also [`Weak::upgrade_in_event_loop`]
 ///
 /// # Example
 /// ```rust
 /// slint::slint! { export component MyApp inherits Window { in property <int> foo; /* ... */ } }
-/// # i_slint_backend_testing::init();
+/// # i_slint_backend_testing::init_no_event_loop();
 /// let handle = MyApp::new().unwrap();
 /// let handle_weak = handle.as_weak();
 /// # return; // don't run the event loop in examples
 /// let thread = std::thread::spawn(move || {
 ///     // ... Do some computation in the thread
 ///     let foo = 42;
 ///      // now forward the data to the main thread using invoke_from_event_loop
```

### Comparing `slint-1.6.0a6/internal/core/callbacks.rs` & `slint-1.6.0a7/internal/core/callbacks.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core/component_factory.rs` & `slint-1.6.0a7/internal/core/component_factory.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core/context.rs` & `slint-1.6.0a7/internal/core/context.rs`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,46 @@
 // Copyright © SixtyFPS GmbH <info@slint.dev>
 // SPDX-License-Identifier: GPL-3.0-only OR LicenseRef-Slint-Royalty-free-1.2 OR LicenseRef-Slint-commercial
 
 use crate::api::PlatformError;
 use crate::platform::{EventLoopProxy, Platform};
 #[cfg(all(not(feature = "std"), feature = "unsafe-single-threaded"))]
 use crate::thread_local;
+use crate::Property;
 #[cfg(not(feature = "std"))]
 use alloc::boxed::Box;
 use alloc::rc::Rc;
 
 thread_local! {
     pub(crate) static GLOBAL_CONTEXT : once_cell::unsync::OnceCell<SlintContext>
         = once_cell::unsync::OnceCell::new()
 }
 
 pub(crate) struct SlintContextInner {
     pub(crate) platform: Box<dyn Platform>,
     pub(crate) window_count: core::cell::RefCell<isize>,
+    /// This property is read by all translations, and marked dirty when the language change
+    /// so that every translated string gets re-translated
+    pub(crate) translations_dirty: core::pin::Pin<Box<Property<()>>>,
 }
 
 /// This context is meant to hold the state and the backend.
 /// Currently it is not possible to have several platform at the same time in one process, but in the future it might be.
 /// See issue #4294
 #[derive(Clone)]
 pub struct SlintContext(pub(crate) Rc<SlintContextInner>);
 
 impl SlintContext {
     /// Create a new context with a given platform
     pub fn new(platform: Box<dyn Platform + 'static>) -> Self {
-        Self(Rc::new(SlintContextInner { platform, window_count: 0.into() }))
+        Self(Rc::new(SlintContextInner {
+            platform,
+            window_count: 0.into(),
+            translations_dirty: Box::pin(Property::new_named((), "SlintContext::translations")),
+        }))
     }
 
     /// Return an event proxy
     // FIXME: Make EvenLoopProxy clonable, and maybe wrap in a struct
     pub fn event_loop_proxy(&self) -> Option<Box<dyn EventLoopProxy>> {
         self.0.platform.new_event_loop_proxy()
     }
```

### Comparing `slint-1.6.0a6/internal/core/future.rs` & `slint-1.6.0a7/internal/core/future.rs`

 * *Files 1% similar despite different names*

```diff
@@ -153,15 +153,15 @@
 /// may not work. To overcome this, these futures should be executed in a thread where the specific
 /// runtime is running.
 ///
 /// For Tokio, this can be achieved by awaiting [tokio::spawn](https://docs.rs/tokio/latest/tokio/task/fn.spawn.html)
 /// in the future passed to slint::spawn_local.
 ///
 /// ```rust
-/// # i_slint_backend_testing::init_with_event_loop();
+/// # i_slint_backend_testing::init_integration_test();
 /// // In your main function, create a runtime that runs on the other threads
 /// let tokio_runtime = tokio::runtime::Runtime::new().unwrap();
 ///
 /// // ...
 /// // Within the UI thread (for example in a callback handler)
 /// slint::spawn_local(async move {
 ///     let result = tokio_runtime.spawn(async move {
```

### Comparing `slint-1.6.0a6/internal/core/graphics/bitmapfont.rs` & `slint-1.6.0a7/internal/core/graphics/bitmapfont.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core/graphics/border_radius.rs` & `slint-1.6.0a7/internal/core/graphics/border_radius.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core/graphics/boxshadowcache.rs` & `slint-1.6.0a7/internal/core/graphics/boxshadowcache.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core/graphics/brush.rs` & `slint-1.6.0a7/internal/core/graphics/brush.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core/graphics/color.rs` & `slint-1.6.0a7/internal/core/graphics/color.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core/graphics/image/cache.rs` & `slint-1.6.0a7/internal/core/graphics/image/cache.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core/graphics/image/htmlimage.rs` & `slint-1.6.0a7/internal/core/graphics/image/htmlimage.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core/graphics/image/svg.rs` & `slint-1.6.0a7/internal/core/graphics/image/svg.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core/graphics/image.rs` & `slint-1.6.0a7/internal/core/graphics/image.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core/graphics/path.rs` & `slint-1.6.0a7/internal/core/graphics/path.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core/graphics/rendering_metrics_collector.rs` & `slint-1.6.0a7/internal/core/graphics/rendering_metrics_collector.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core/graphics.rs` & `slint-1.6.0a7/internal/core/graphics.rs`

 * *Files 3% similar despite different names*

```diff
@@ -194,14 +194,23 @@
     #[cfg(cbindgen)]
     #[repr(C)]
     struct Point {
         x: f32,
         y: f32,
     }
 
+    /// Expand Box2D so that cbindgen can see it.
+    #[cfg(cbindgen)]
+    #[repr(C)]
+    struct Box2D<T, U> {
+        min: euclid::Point2D<T>,
+        max: euclid::Point2D<T>,
+        _unit: std::marker::PhantomData<U>,
+    }
+
     #[cfg(feature = "std")]
     pub use super::path::ffi::*;
 
     /// Conversion function used by C++ platform API layer to
     /// convert the PhysicalSize used in the Rust WindowAdapter API
     /// to the ffi.
     pub fn physical_size_from_api(
```

### Comparing `slint-1.6.0a6/internal/core/input.rs` & `slint-1.6.0a7/internal/core/input.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core/item_focus.rs` & `slint-1.6.0a7/internal/core/item_focus.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core/item_rendering.rs` & `slint-1.6.0a7/internal/core/item_rendering.rs`

 * *Files 7% similar despite different names*

```diff
@@ -392,14 +392,17 @@
         radius: LogicalBorderRadius,
         border_width: LogicalLength,
     ) -> bool;
     /// Get the current clip bounding box in the current transformed coordinate.
     fn get_current_clip(&self) -> LogicalRect;
 
     fn translate(&mut self, distance: LogicalVector);
+    fn translation(&self) -> LogicalVector {
+        unimplemented!()
+    }
     fn rotate(&mut self, angle_in_degrees: f32);
     /// Apply the opacity (between 0 and 1) for all following items until the next call to restore_state.
     fn apply_opacity(&mut self, opacity: f32);
 
     fn save_state(&mut self);
     fn restore_state(&mut self);
 
@@ -442,16 +445,129 @@
         Default::default()
     }
 }
 
 /// The cache that needs to be held by the Window for the partial rendering
 pub type PartialRenderingCache = RenderingCache<LogicalRect>;
 
-/// FIXME: Should actually be a region and not just a rectangle
-pub type DirtyRegion = euclid::Box2D<Coord, LogicalPx>;
+/// A region composed of a few rectangles that need to be redrawn.
+#[derive(Default, Clone, Debug)]
+pub struct DirtyRegion {
+    rectangles: [euclid::Box2D<Coord, LogicalPx>; Self::MAX_COUNT],
+    count: usize,
+}
+
+impl DirtyRegion {
+    /// The maximum number of rectangles that can be stored in a DirtyRegion
+    pub(crate) const MAX_COUNT: usize = 3;
+
+    /// An iterator over the part of the region (they can overlap)
+    pub fn iter(&self) -> impl Iterator<Item = euclid::Box2D<Coord, LogicalPx>> + '_ {
+        (0..self.count).map(|x| self.rectangles[x])
+    }
+
+    /// Add a rectangle to the region.
+    ///
+    /// Note that if the region becomes too complex, it might be simplified by being bigger than the actual union.
+    pub fn add_rect(&mut self, rect: LogicalRect) {
+        self.add_box(rect.to_box2d());
+    }
+
+    /// Add a box to the region
+    ///
+    /// Note that if the region becomes too complex, it might be simplified by being bigger than the actual union.
+    pub fn add_box(&mut self, b: euclid::Box2D<Coord, LogicalPx>) {
+        if b.is_empty() {
+            return;
+        }
+        let mut i = 0;
+        while i < self.count {
+            let r = &self.rectangles[i];
+            if r.contains_box(&b) {
+                // the rectangle is already in the union
+                return;
+            } else if b.contains_box(&r) {
+                self.rectangles.swap(i, self.count - 1);
+                self.count -= 1;
+                continue;
+            }
+            i += 1;
+        }
+
+        if self.count < Self::MAX_COUNT {
+            self.rectangles[self.count] = b;
+            self.count += 1;
+            return;
+        } else {
+            let best_merge = (0..self.count)
+                .map(|i| (i, self.rectangles[i].union(&b).area() - self.rectangles[i].area()))
+                .min_by(|a, b| PartialOrd::partial_cmp(&a.1, &b.1).unwrap())
+                .expect("There should always be rectangles")
+                .0;
+            self.rectangles[best_merge] = self.rectangles[best_merge].union(&b);
+        }
+    }
+
+    /// Make an union of two regions.
+    ///
+    /// Note that if the region becomes too complex, it might be simplified by being bigger than the actual union
+    #[must_use]
+    pub fn union(&self, other: &Self) -> Self {
+        let mut s = self.clone();
+        for o in other.iter() {
+            s.add_box(o)
+        }
+        s
+    }
+
+    /// Bounding rectangle of the region.
+    #[must_use]
+    pub fn bounding_rect(&self) -> LogicalRect {
+        if self.count == 0 {
+            return Default::default();
+        }
+        let mut r = self.rectangles[0];
+        for i in 1..self.count {
+            r = r.union(&self.rectangles[i]);
+        }
+        r.to_rect()
+    }
+
+    /// Intersection of a region and a rectangle.
+    #[must_use]
+    pub fn intersection(&self, other: LogicalRect) -> DirtyRegion {
+        let mut ret = self.clone();
+        let other = other.to_box2d();
+        let mut i = 0;
+        while i < ret.count {
+            if let Some(x) = ret.rectangles[i].intersection(&other) {
+                ret.rectangles[i] = x;
+            } else {
+                ret.rectangles.swap(i, ret.count);
+                ret.count -= 1;
+                continue;
+            }
+            i += 1;
+        }
+        ret
+    }
+
+    fn draw_intersects(&self, clipped_geom: LogicalRect) -> bool {
+        let b = clipped_geom.to_box2d();
+        self.iter().any(|r| r.intersects(&b))
+    }
+}
+
+impl From<LogicalRect> for DirtyRegion {
+    fn from(value: LogicalRect) -> Self {
+        let mut s = Self::default();
+        s.add_rect(value);
+        s
+    }
+}
 
 /// Put this structure in the renderer to help with partial rendering
 pub struct PartialRenderer<'a, T> {
     cache: &'a RefCell<PartialRenderingCache>,
     /// The region of the screen which is considered dirty and that should be repainted
     pub dirty_region: DirtyRegion,
     /// The actual renderer which the drawing call will be forwarded to
@@ -465,15 +581,20 @@
         initial_dirty_region: DirtyRegion,
         actual_renderer: T,
     ) -> Self {
         Self { cache, dirty_region: initial_dirty_region, actual_renderer }
     }
 
     /// Visit the tree of item and compute what are the dirty regions
-    pub fn compute_dirty_regions(&mut self, component: &ItemTreeRc, origin: LogicalPoint) {
+    pub fn compute_dirty_regions(
+        &mut self,
+        component: &ItemTreeRc,
+        origin: LogicalPoint,
+        size: LogicalSize,
+    ) {
         #[derive(Clone, Copy)]
         struct ComputeDirtyRegionState {
             offset: euclid::Vector2D<Coord, LogicalPx>,
             old_offset: euclid::Vector2D<Coord, LogicalPx>,
             clipped: LogicalRect,
             must_refresh_children: bool,
         }
@@ -558,29 +679,29 @@
                         ItemVisitorResult::Continue(new_state)
                     }
                 }
             },
             ComputeDirtyRegionState {
                 offset: origin.to_vector(),
                 old_offset: origin.to_vector(),
-                clipped: euclid::rect(0 as Coord, 0 as Coord, Coord::MAX, Coord::MAX),
+                clipped: LogicalRect::from_size(size),
                 must_refresh_children: false,
             },
         );
     }
 
     fn mark_dirty_rect(
         &mut self,
         rect: LogicalRect,
         offset: euclid::Vector2D<Coord, LogicalPx>,
         clip_rect: &LogicalRect,
     ) {
         if !rect.is_empty() {
             if let Some(rect) = rect.translate(offset).intersection(clip_rect) {
-                self.dirty_region = self.dirty_region.union(&rect.to_box2d());
+                self.dirty_region.add_rect(rect);
             }
         }
     }
 
     fn do_rendering(
         cache: &RefCell<PartialRenderingCache>,
         rendering_data: &CachedRenderingData,
@@ -658,18 +779,20 @@
                 let geom = cache_entry.data;
                 rendering_data.cache_index.set(cache.insert(cache_entry));
                 rendering_data.cache_generation.set(cache.generation());
                 geom
             }
         };
 
-        //let clip = self.get_current_clip().intersection(&self.dirty_region.to_rect());
-        //let draw = clip.map_or(false, |r| r.intersects(&item_geometry));
-        //FIXME: the dirty_region is in global coordinate but item_geometry and current_clip is not
-        let draw = self.get_current_clip().intersects(&item_geometry);
+        let clipped_geom = self.get_current_clip().intersection(&item_geometry);
+        let draw = clipped_geom.map_or(false, |clipped_geom| {
+            let clipped_geom = clipped_geom.translate(self.translation());
+            self.dirty_region.draw_intersects(clipped_geom)
+        });
+
         (draw, item_geometry)
     }
 
     forward_rendering_call!(fn draw_rectangle(Rectangle));
     forward_rendering_call2!(fn draw_border_rectangle(dyn RenderBorderRectangle));
     forward_rendering_call2!(fn draw_image(dyn RenderImage));
     forward_rendering_call!(fn draw_text(Text));
@@ -693,14 +816,17 @@
     fn get_current_clip(&self) -> LogicalRect {
         self.actual_renderer.get_current_clip()
     }
 
     fn translate(&mut self, distance: LogicalVector) {
         self.actual_renderer.translate(distance)
     }
+    fn translation(&self) -> LogicalVector {
+        self.actual_renderer.translation()
+    }
 
     fn rotate(&mut self, angle_in_degrees: f32) {
         self.actual_renderer.rotate(angle_in_degrees)
     }
 
     fn apply_opacity(&mut self, opacity: f32) {
         self.actual_renderer.apply_opacity(opacity)
```

### Comparing `slint-1.6.0a6/internal/core/item_tree.rs` & `slint-1.6.0a7/internal/core/item_tree.rs`

 * *Files 0% similar despite different names*

```diff
@@ -103,21 +103,21 @@
     pub item_geometry:
         extern "C" fn(core::pin::Pin<VRef<ItemTreeVTable>>, item_index: u32) -> LogicalRect,
 
     /// Returns the accessible role for a given item
     pub accessible_role:
         extern "C" fn(core::pin::Pin<VRef<ItemTreeVTable>>, item_index: u32) -> AccessibleRole,
 
-    /// Returns the accessible property
+    /// Returns the accessible property via the `result`. Returns true if such a property exists.
     pub accessible_string_property: extern "C" fn(
         core::pin::Pin<VRef<ItemTreeVTable>>,
         item_index: u32,
         what: AccessibleStringProperty,
         result: &mut SharedString,
-    ),
+    ) -> bool,
 
     /// Executes an accessibility action.
     pub accessibility_action: extern "C" fn(
         core::pin::Pin<VRef<ItemTreeVTable>>,
         item_index: u32,
         action: &AccessibilityAction,
     ),
@@ -339,19 +339,19 @@
         let comp_ref_pin = vtable::VRc::borrow_pin(&self.item_tree);
         comp_ref_pin.as_ref().accessible_role(self.index)
     }
 
     pub fn accessible_string_property(
         &self,
         what: crate::accessibility::AccessibleStringProperty,
-    ) -> SharedString {
+    ) -> Option<SharedString> {
         let comp_ref_pin = vtable::VRc::borrow_pin(&self.item_tree);
         let mut result = Default::default();
-        comp_ref_pin.as_ref().accessible_string_property(self.index, what, &mut result);
-        result
+        let ok = comp_ref_pin.as_ref().accessible_string_property(self.index, what, &mut result);
+        ok.then_some(result)
     }
 
     pub fn accessible_action(&self, action: &crate::accessibility::AccessibilityAction) {
         let comp_ref_pin = vtable::VRc::borrow_pin(&self.item_tree);
         comp_ref_pin.as_ref().accessibility_action(self.index, action);
     }
 
@@ -1144,15 +1144,16 @@
         }
 
         fn accessible_string_property(
             self: Pin<&Self>,
             _: u32,
             _: AccessibleStringProperty,
             _: &mut SharedString,
-        ) {
+        ) -> bool {
+            false
         }
 
         fn window_adapter(
             self: Pin<&Self>,
             _do_create: bool,
             _result: &mut Option<WindowAdapterRc>,
         ) {
```

### Comparing `slint-1.6.0a6/internal/core/items/component_container.rs` & `slint-1.6.0a7/internal/core/items/component_container.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core/items/flickable.rs` & `slint-1.6.0a7/internal/core/items/flickable.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core/items/image.rs` & `slint-1.6.0a7/internal/core/items/image.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core/items/path.rs` & `slint-1.6.0a7/internal/core/items/path.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core/items/text.rs` & `slint-1.6.0a7/internal/core/items/text.rs`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 This module contains the builtin text related items.
 
 When adding an item or a property, it needs to be kept in sync with different place.
 Lookup the [`crate::items`] module documentation.
 */
 use super::{
     InputType, Item, ItemConsts, ItemRc, KeyEventResult, KeyEventType, PointArg,
-    PointerEventButton, RenderingResult, TextHorizontalAlignment, TextOverflow,
+    PointerEventButton, RenderingResult, TextHorizontalAlignment, TextOverflow, TextStrokeStyle,
     TextVerticalAlignment, TextWrap, VoidArg,
 };
 use crate::graphics::{Brush, Color, FontRequest};
 use crate::input::{
     key_codes, FocusEvent, FocusEventResult, InputEventFilterResult, InputEventResult, KeyEvent,
     KeyboardModifiers, MouseEvent, StandardShortcut, TextShortcut,
 };
@@ -47,14 +47,17 @@
     pub font_italic: Property<bool>,
     pub color: Property<Brush>,
     pub horizontal_alignment: Property<TextHorizontalAlignment>,
     pub vertical_alignment: Property<TextVerticalAlignment>,
     pub wrap: Property<TextWrap>,
     pub overflow: Property<TextOverflow>,
     pub letter_spacing: Property<LogicalLength>,
+    pub stroke: Property<Brush>,
+    pub stroke_width: Property<LogicalLength>,
+    pub stroke_style: Property<TextStrokeStyle>,
     pub width: Property<LogicalLength>,
     pub height: Property<LogicalLength>,
     pub cached_rendering_data: CachedRenderingData,
 }
 
 impl Item for Text {
     fn init(self: Pin<&Self>, _self_rc: &ItemRc) {}
@@ -1472,15 +1475,15 @@
     /// Setting the focus will show the virtual keyboard, otherwise we should make sure that the keyboard is shown if it was hidden by the user
     fn ensure_focus_and_ime(
         self: Pin<&Self>,
         window_adapter: &Rc<dyn WindowAdapter>,
         self_rc: &ItemRc,
     ) {
         if !self.has_focus() {
-            WindowInner::from_pub(window_adapter.window()).set_focus_item(self_rc);
+            WindowInner::from_pub(window_adapter.window()).set_focus_item(self_rc, true);
         } else if !self.read_only() {
             if let Some(w) = window_adapter.internal(crate::InternalToken) {
                 w.input_method_request(InputMethodRequest::Enable(
                     self.ime_properties(window_adapter, self_rc),
                 ));
             }
         }
```

### Comparing `slint-1.6.0a6/internal/core/items.rs` & `slint-1.6.0a7/internal/core/items.rs`

 * *Files 0% similar despite different names*

```diff
@@ -771,15 +771,15 @@
     fn input_event(
         self: Pin<&Self>,
         event: MouseEvent,
         window_adapter: &Rc<dyn WindowAdapter>,
         self_rc: &ItemRc,
     ) -> InputEventResult {
         if self.enabled() && matches!(event, MouseEvent::Pressed { .. }) && !self.has_focus() {
-            WindowInner::from_pub(window_adapter.window()).set_focus_item(self_rc);
+            WindowInner::from_pub(window_adapter.window()).set_focus_item(self_rc, true);
             InputEventResult::EventAccepted
         } else {
             InputEventResult::EventIgnored
         }
     }
 
     fn key_event(
```

### Comparing `slint-1.6.0a6/internal/core/layout.rs` & `slint-1.6.0a7/internal/core/layout.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core/lengths.rs` & `slint-1.6.0a7/internal/core/lengths.rs`

 * *Files 3% similar despite different names*

```diff
@@ -92,7 +92,11 @@
 pub fn logical_point_from_api(position: crate::api::LogicalPosition) -> LogicalPoint {
     position.to_euclid()
 }
 
 pub fn logical_position_to_api(pos: LogicalPoint) -> crate::api::LogicalPosition {
     crate::api::LogicalPosition::from_euclid(pos)
 }
+
+pub fn logical_size_to_api(size: LogicalSize) -> crate::api::LogicalSize {
+    crate::api::LogicalSize::from_euclid(size)
+}
```

### Comparing `slint-1.6.0a6/internal/core/lib.rs` & `slint-1.6.0a7/internal/core/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core/model/adapters.rs` & `slint-1.6.0a7/internal/core/model/adapters.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core/model/model_peer.rs` & `slint-1.6.0a7/internal/core/model/model_peer.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core/model.rs` & `slint-1.6.0a7/internal/core/model.rs`

 * *Files 0% similar despite different names*

```diff
@@ -542,15 +542,15 @@
 ///   [`Model`] trait, such as [`VecModel`] or your own implementation.
 /// * If you have your model already in an `Rc`, then you can use the [`From`] trait
 ///   to convert from `Rc<dyn Model<Data = T>>` to `ModelRc`.
 ///
 /// ## Example
 ///
 /// ```rust
-/// # i_slint_backend_testing::init();
+/// # i_slint_backend_testing::init_no_event_loop();
 /// use slint::{slint, SharedString, ModelRc, Model, VecModel};
 /// use std::rc::Rc;
 /// slint!{
 ///     import { Button } from "std-widgets.slint";
 ///     export component Example {
 ///         callback add_item <=> btn.clicked;
 ///         in property <[string]> the_model;
```

### Comparing `slint-1.6.0a6/internal/core/platform.rs` & `slint-1.6.0a7/internal/core/platform.rs`

 * *Files 1% similar despite different names*

```diff
@@ -217,14 +217,15 @@
 /// as advance the state of any active animations.
 ///
 /// This function should be called before rendering or processing input event, at the
 /// beginning of each event loop iteration.
 pub fn update_timers_and_animations() {
     crate::animations::update_animations();
     crate::timers::TimerList::maybe_activate_timers(crate::animations::Instant::now());
+    crate::properties::ChangeTracker::run_change_handlers();
 }
 
 /// Returns the duration before the next timer is expected to be activated. This is the
 /// largest amount of time that you can wait before calling [`update_timers_and_animations()`].
 ///
 /// `None` is returned if there is no active timer.
 ///
```

### Comparing `slint-1.6.0a6/internal/core/properties/ffi.rs` & `slint-1.6.0a7/internal/core/properties/ffi.rs`

 * *Files 20% similar despite different names*

```diff
@@ -215,14 +215,25 @@
     from: Color,
     to: Color,
     animation_data: &PropertyAnimation,
 ) {
     c_set_animated_value(handle, from, to, animation_data);
 }
 
+/// Internal function to set up a property animation to the specified target value for a brush property.
+#[no_mangle]
+pub unsafe extern "C" fn slint_property_set_animated_value_brush(
+    handle: &PropertyHandleOpaque,
+    from: &Brush,
+    to: &Brush,
+    animation_data: &PropertyAnimation,
+) {
+    c_set_animated_value(handle, from.clone(), to.clone(), animation_data);
+}
+
 unsafe fn c_set_animated_binding<T: InterpolatedPropertyValue + Clone>(
     handle: &PropertyHandleOpaque,
     binding: extern "C" fn(*mut c_void, *mut T),
     user_data: *mut c_void,
     drop_user_data: Option<extern "C" fn(*mut c_void)>,
     animation_data: Option<&PropertyAnimation>,
     transition_data: Option<
@@ -446,12 +457,94 @@
 
 /// Destroy handle
 #[no_mangle]
 pub unsafe extern "C" fn slint_property_tracker_drop(handle: *mut PropertyTrackerOpaque) {
     core::ptr::drop_in_place(handle as *mut PropertyTracker);
 }
 
+/// Construct a ChangeTracker
+#[no_mangle]
+pub unsafe extern "C" fn slint_change_tracker_construct(ct: *mut ChangeTracker) {
+    core::ptr::write(ct, ChangeTracker::default());
+}
+
+/// Drop a ChangeTracker
+#[no_mangle]
+pub unsafe extern "C" fn slint_change_tracker_drop(ct: *mut ChangeTracker) {
+    core::ptr::drop_in_place(ct);
+}
+
+/// initialize the change tracker
+#[no_mangle]
+pub unsafe extern "C" fn slint_change_tracker_init(
+    ct: &ChangeTracker,
+    user_data: *mut c_void,
+    drop_user_data: extern "C" fn(user_data: *mut c_void),
+    eval_fn: extern "C" fn(user_data: *mut c_void) -> bool,
+    notify_fn: extern "C" fn(user_data: *mut c_void),
+) {
+    #[allow(non_camel_case_types)]
+    struct C_ChangeTrackerInner {
+        user_data: *mut c_void,
+        drop_user_data: extern "C" fn(user_data: *mut c_void),
+        eval_fn: extern "C" fn(user_data: *mut c_void) -> bool,
+        notify_fn: extern "C" fn(user_data: *mut c_void),
+    }
+    impl Drop for C_ChangeTrackerInner {
+        fn drop(&mut self) {
+            (self.drop_user_data)(self.user_data);
+        }
+    }
+
+    unsafe fn drop(_self: *mut BindingHolder) {
+        core::mem::drop(Box::from_raw(_self as *mut BindingHolder<C_ChangeTrackerInner>));
+    }
+
+    unsafe fn evaluate(_self: *mut BindingHolder, _value: *mut ()) -> BindingResult {
+        let pinned_holder = Pin::new_unchecked(&*_self);
+        let _self = _self as *mut BindingHolder<C_ChangeTrackerInner>;
+        let inner = core::ptr::addr_of_mut!((*_self).binding).as_mut().unwrap();
+        let notify =
+            super::CURRENT_BINDING.set(Some(pinned_holder), || (inner.eval_fn)(inner.user_data));
+        if notify {
+            (inner.notify_fn)(inner.user_data);
+        }
+        BindingResult::KeepBinding
+    }
+
+    const VT: &'static BindingVTable = &BindingVTable {
+        drop,
+        evaluate,
+        mark_dirty: ChangeTracker::mark_dirty,
+        intercept_set: |_, _| false,
+        intercept_set_binding: |_, _| false,
+    };
+
+    ct.clear();
+
+    let inner = C_ChangeTrackerInner { user_data, drop_user_data, eval_fn, notify_fn };
+
+    let holder = BindingHolder {
+        dependencies: Cell::new(0),
+        dep_nodes: Default::default(),
+        vtable: VT,
+        dirty: Cell::new(false),
+        is_two_way_binding: false,
+        pinned: PhantomPinned,
+        binding: inner,
+        #[cfg(slint_debug_property)]
+        debug_name: "<ChangeTracker>".into(),
+    };
+
+    let raw = Box::into_raw(Box::new(holder));
+    ct.set_internal(raw as *mut BindingHolder);
+
+    let pinned_holder = Pin::new_unchecked(&*(raw as *mut BindingHolder));
+    let inner = core::ptr::addr_of_mut!((*raw).binding).as_mut().unwrap();
+    super::CURRENT_BINDING.set(Some(pinned_holder), || (inner.eval_fn)(inner.user_data));
+}
+
 /// return the current animation tick for the `animation-tick` function
 #[no_mangle]
 pub extern "C" fn slint_animation_tick() -> u64 {
     crate::animations::animation_tick()
 }
```

### Comparing `slint-1.6.0a6/internal/core/properties/properties_animations.rs` & `slint-1.6.0a7/internal/core/properties/properties_animations.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core/properties.rs` & `slint-1.6.0a7/internal/core/properties.rs`

 * *Files 4% similar despite different names*

```diff
@@ -120,14 +120,49 @@
             if let Some(next) = ((*from).0.get() as *const DependencyNode<T>).as_ref() {
                 debug_assert_eq!(from as *const _, next.prev.get() as *const _);
                 next.debug_assert_valid();
                 next.prev.set(to as *const _);
                 next.debug_assert_valid();
             }
         }
+
+        /// Swap two list head
+        pub fn swap(from: Pin<&Self>, to: Pin<&Self>) {
+            Cell::swap(&from.0, &to.0);
+            unsafe {
+                if let Some(n) = from.0.get().as_ref() {
+                    debug_assert_eq!(n.prev.get() as *const _, &to.0 as *const _);
+                    n.prev.set(&from.0 as *const _);
+                    n.debug_assert_valid();
+                }
+
+                if let Some(n) = to.0.get().as_ref() {
+                    debug_assert_eq!(n.prev.get() as *const _, &from.0 as *const _);
+                    n.prev.set(&to.0 as *const _);
+                    n.debug_assert_valid();
+                }
+            }
+        }
+
+        /// Return true is the list is empty
+        pub fn is_empty(&self) -> bool {
+            self.0.get().is_null()
+        }
+
+        /// Remove all the nodes from the list;
+        pub fn clear(self: Pin<&Self>) {
+            unsafe {
+                if let Some(n) = self.0.get().as_ref() {
+                    n.debug_assert_valid();
+                    n.prev.set(core::ptr::null());
+                }
+            }
+            self.0.set(core::ptr::null());
+        }
+
         pub unsafe fn drop(_self: *mut Self) {
             if let Some(next) = ((*_self).0.get() as *const DependencyNode<T>).as_ref() {
                 debug_assert_eq!(_self as *const _, next.prev.get() as *const _);
                 next.debug_assert_valid();
                 next.prev.set(core::ptr::null());
                 next.debug_assert_valid();
             }
@@ -1273,14 +1308,16 @@
     p2_2.set(9);
     assert_eq!(p1_1.as_ref().get(), 9);
     assert_eq!(p1_2.as_ref().get(), 9);
     assert_eq!(p2_1.as_ref().get(), 9);
     assert_eq!(p2_2.as_ref().get(), 9);
 }
 
+mod change_tracker;
+pub use change_tracker::*;
 mod properties_animations;
 pub use crate::items::StateInfo;
 pub use properties_animations::*;
 
 struct StateInfoBinding<F> {
     dirty_time: Cell<Option<crate::animations::Instant>>,
     binding: F,
@@ -1318,24 +1355,24 @@
             property.debug_name.borrow().as_str(),
         )
     }
 }
 
 #[doc(hidden)]
 pub trait PropertyDirtyHandler {
-    fn notify(&self);
+    fn notify(self: Pin<&Self>);
 }
 
 impl PropertyDirtyHandler for () {
-    fn notify(&self) {}
+    fn notify(self: Pin<&Self>) {}
 }
 
 impl<F: Fn()> PropertyDirtyHandler for F {
-    fn notify(&self) {
-        self()
+    fn notify(self: Pin<&Self>) {
+        (self.get_ref())()
     }
 }
 
 /// This structure allow to run a closure that queries properties, and can report
 /// if any property we accessed have become dirty
 pub struct PropertyTracker<DirtyHandler = ()> {
     holder: BindingHolder<DirtyHandler>,
@@ -1458,15 +1495,15 @@
     pub fn new_with_dirty_handler(handler: DirtyHandler) -> Self {
         /// Safety: _self must be a pointer to a `BindingHolder<DirtyHandler>`
         unsafe fn mark_dirty<B: PropertyDirtyHandler>(
             _self: *const BindingHolder,
             was_dirty: bool,
         ) {
             if !was_dirty {
-                ((*(_self as *const BindingHolder<B>)).binding).notify();
+                Pin::new_unchecked(&(*(_self as *const BindingHolder<B>)).binding).notify();
             }
         }
 
         trait HasBindingVTable {
             const VT: &'static BindingVTable;
         }
         impl<B: PropertyDirtyHandler> HasBindingVTable for B {
```

### Comparing `slint-1.6.0a6/internal/core/renderer.rs` & `slint-1.6.0a7/internal/core/renderer.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core/rtti.rs` & `slint-1.6.0a7/internal/core/rtti.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core/sharedvector.rs` & `slint-1.6.0a7/internal/core/sharedvector.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core/slice.rs` & `slint-1.6.0a7/internal/core/slice.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core/software_renderer/draw_functions.rs` & `slint-1.6.0a7/internal/core/software_renderer/draw_functions.rs`

 * *Files 8% similar despite different names*

```diff
@@ -4,46 +4,45 @@
 #![allow(clippy::identity_op)] // We use x + 0 a lot here for symmetry
 
 //! This is the module for the functions that are drawing the pixels
 //! on the line buffer
 
 use super::{PhysicalLength, PhysicalRect};
 use crate::graphics::{PixelFormat, Rgb8Pixel};
-use crate::lengths::{PointLengths, RectLengths, SizeLengths};
+use crate::lengths::{PointLengths, SizeLengths};
 use crate::software_renderer::fixed::Fixed;
 use crate::Color;
 use derive_more::{Add, Mul, Sub};
 use integer_sqrt::IntegerSquareRoot;
 
 /// Draw one line of the texture in the line buffer
+///
 pub(super) fn draw_texture_line(
     span: &PhysicalRect,
     line: PhysicalLength,
     texture: &super::SceneTexture,
     line_buffer: &mut [impl TargetPixel],
+    extra_clip: i16,
 ) {
     let super::SceneTexture {
         data,
         format,
         pixel_stride,
         extra: super::SceneTextureExtra { colorize, alpha, rotation, dx, dy, off_x, off_y },
     } = *texture;
-    let span_size = span.size.cast::<usize>();
 
     let source_size = texture.source_size().cast::<i32>();
+    let len = line_buffer.len();
+    let y = line - span.origin.y_length();
+    let y = if rotation.mirror_width() { span.size.height - y.get() - 1 } else { y.get() } as i32;
 
-    let line_buffer = &mut line_buffer[span.origin.x as usize..];
-
-    let y = (line - span.origin.y_length()).cast::<usize>();
-    let y = if rotation.mirror_width() { span_size.height - y.get() - 1 } else { y.get() } as i32;
-
-    let off_x = Fixed::<i32, 8>::from_fixed(off_x);
     let off_y = Fixed::<i32, 8>::from_fixed(off_y);
     let dx = Fixed::<i32, 8>::from_fixed(dx);
     let dy = Fixed::<i32, 8>::from_fixed(dy);
+    let off_x = Fixed::<i32, 8>::from_fixed(off_x) + dx * extra_clip as i32;
 
     if !rotation.is_transpose() {
         let mut delta = dx;
         // The position where to start in the image array for a this row
         let mut init = Fixed::from_integer((off_y + dy * y).truncate() % source_size.height)
             * pixel_stride as i32;
 
@@ -54,16 +53,15 @@
         // The position in image pixel where to get the image
         let mut pos;
         // the end index in the target buffer
         let mut end;
         // the accumulated error in image pixels
         let mut acc_err;
         if rotation.mirror_height() {
-            let o = (off_x + (delta * (span_size.width as i32 - 1)))
-                % Fixed::from_integer(source_size.width);
+            let o = (off_x + (delta * (len as i32 - 1))) % Fixed::from_integer(source_size.width);
             pos = init + o;
             init += Fixed::from_integer(source_size.width);
             end = (o / delta) as usize + 1;
             acc_err = -delta + o % delta;
             delta = -delta;
             remainder = -remainder;
         } else {
@@ -72,17 +70,17 @@
             end = ((Fixed::from_integer(source_size.width) - o) / delta) as usize;
             acc_err = (Fixed::from_integer(source_size.width) - o) % delta;
             if acc_err != Fixed::default() {
                 acc_err = delta - acc_err;
                 end += 1;
             }
         }
-        end = end.min(span_size.width);
+        end = end.min(len);
         let mut begin = 0;
-        while begin < span_size.width {
+        while begin < len {
             fetch_blend_pixel(
                 &mut line_buffer[begin..end],
                 format,
                 data,
                 alpha,
                 colorize,
                 #[inline(always)]
@@ -104,15 +102,15 @@
                     acc_err < Fixed::from_integer(0)
                 };
                 if wrap {
                     acc_err += delta;
                     end += 1;
                 }
             };
-            end = end.min(span_size.width);
+            end = end.min(len);
         }
     } else {
         let bpp = format.bpp();
         let col = off_x + dx * y;
         let col = (col.truncate() % source_size.width) as usize * bpp;
         let stride = pixel_stride as usize * bpp;
         let mut row_delta = dy;
@@ -120,32 +118,32 @@
         let mut remainder = Fixed::from_integer(source_size.height) % row_delta;
         let mut end;
         let mut row_init = Fixed::default();
         let mut row;
         let mut acc_err;
         if rotation.mirror_height() {
             row_init = Fixed::from_integer(source_size.height);
-            row = (off_y + (row_delta * (span_size.width as i32 - 1)))
-                % Fixed::from_integer(source_size.height);
+            row =
+                (off_y + (row_delta * (len as i32 - 1))) % Fixed::from_integer(source_size.height);
             end = (row / row_delta) as usize + 1;
             acc_err = -row_delta + row % row_delta;
             row_delta = -row_delta;
             remainder = -remainder;
         } else {
             row = off_y % Fixed::from_integer(source_size.height);
             end = ((Fixed::from_integer(source_size.height) - row) / row_delta) as usize;
             acc_err = (Fixed::from_integer(source_size.height) - row) % row_delta;
             if acc_err != Fixed::default() {
                 acc_err = row_delta - acc_err;
                 end += 1;
             }
         };
-        end = end.min(span_size.width);
+        end = end.min(len);
         let mut begin = 0;
-        while begin < span_size.width {
+        while begin < len {
             fetch_blend_pixel(
                 &mut line_buffer[begin..end],
                 format,
                 data,
                 alpha,
                 colorize,
                 #[inline(always)]
@@ -167,15 +165,15 @@
                     acc_err < Fixed::from_integer(0)
                 };
                 if wrap {
                     acc_err += row_delta;
                     end += 1;
                 }
             };
-            end = end.min(span_size.width);
+            end = end.min(len);
         }
     };
 
     fn fetch_blend_pixel(
         line_buffer: &mut [impl TargetPixel],
         format: PixelFormat,
         data: &[u8],
@@ -279,14 +277,16 @@
 /// draw one line of the rounded rectangle in the line buffer
 #[allow(clippy::unnecessary_cast)] // Coord
 pub(super) fn draw_rounded_rectangle_line(
     span: &PhysicalRect,
     line: PhysicalLength,
     rr: &super::RoundedRectangle,
     line_buffer: &mut [impl TargetPixel],
+    extra_left_clip: i16,
+    extra_right_clip: i16,
 ) {
     /// This is an integer shifted by 4 bits.
     /// Note: this is not a "fixed point" because multiplication and sqrt operation operate to
     /// the shifted integer
     #[derive(Clone, Copy, PartialEq, Ord, PartialOrd, Eq, Add, Sub, Mul)]
     struct Shifted(u32);
     impl Shifted {
@@ -309,15 +309,15 @@
     }
     impl core::ops::Mul for Shifted {
         type Output = Shifted;
         fn mul(self, rhs: Self) -> Self::Output {
             Self(self.0 * rhs.0)
         }
     }
-    let pos_x = span.origin.x as usize;
+    let width = line_buffer.len();
     let y1 = (line - span.origin.y_length()) + rr.top_clip;
     let y2 = (span.origin.y_length() + span.size.height_length() - line) + rr.bottom_clip
         - PhysicalLength::new(1);
     let y = y1.min(y2);
     debug_assert!(y.get() >= 0,);
     let border = Shifted::new(rr.width.get());
     const ONE: Shifted = Shifted::ONE;
@@ -330,15 +330,16 @@
         for x in x1.floor()..x2.ceil() {
             // the coverage is basically how much of the pixel should be used
             let cov = ((ONE + Shifted::new(x) - x1).0 << 8) / (ONE + x2 - x1).0;
             process_pixel(x as usize, cov);
         }
     };
     let rev = |x: Shifted| {
-        (Shifted::new(span.size.width) + Shifted::new(rr.right_clip.get())).saturating_sub(x)
+        (Shifted::new(width) + Shifted::new(rr.right_clip.get() + extra_right_clip))
+            .saturating_sub(x)
     };
     let calculate_xxxx = |r: i16, y: i16| {
         let r = Shifted::new(r);
         // `y` is how far away from the center of the circle the current line is.
         let y = r - Shifted::new(y);
         // Circle equation: x = √(r² - y²)
         // Coordinate from the left edge: x' = r - x
@@ -370,111 +371,113 @@
             (x.3, x.2, x.1, x.0)
         } else {
             (border, border, ZERO, ZERO)
         };
         (x1, x2, x3, x4, rev(x5), rev(x6), rev(x7), rev(x8))
     };
     anti_alias(
-        x1.saturating_sub(Shifted::new(rr.left_clip.get())),
-        x2.saturating_sub(Shifted::new(rr.left_clip.get())),
+        x1.saturating_sub(Shifted::new(rr.left_clip.get() + extra_left_clip)),
+        x2.saturating_sub(Shifted::new(rr.left_clip.get() + extra_left_clip)),
         &mut |x, cov| {
-            if x >= span.size.width as usize {
+            if x >= width {
                 return;
             }
             let c = if border == ZERO { rr.inner_color } else { rr.border_color };
             let col = PremultipliedRgbaColor {
                 alpha: (((c.alpha as u32) * cov as u32) / 255) as u8,
                 red: (((c.red as u32) * cov as u32) / 255) as u8,
                 green: (((c.green as u32) * cov as u32) / 255) as u8,
                 blue: (((c.blue as u32) * cov as u32) / 255) as u8,
             };
-            line_buffer[pos_x + x].blend(col);
+            line_buffer[x].blend(col);
         },
     );
     if y < rr.width {
         // up or down border (x2 .. x7)
-        let l = x2.ceil().saturating_sub(rr.left_clip.get() as u32).min(span.size.width as u32)
-            as usize;
-        let r = x7.floor().min(span.size.width as u32) as usize;
+        let l = x2
+            .ceil()
+            .saturating_sub((rr.left_clip.get() + extra_left_clip) as u32)
+            .min(width as u32) as usize;
+        let r = x7.floor().min(width as u32) as usize;
         if l < r {
-            TargetPixel::blend_slice(&mut line_buffer[pos_x + l..pos_x + r], rr.border_color)
+            TargetPixel::blend_slice(&mut line_buffer[l..r], rr.border_color)
         }
     } else {
         if border > ZERO {
             // 3. draw the border (between x2 and x3)
             if ONE + x2 <= x3 {
                 TargetPixel::blend_slice(
-                    &mut line_buffer[pos_x
-                        + x2.ceil()
-                            .saturating_sub(rr.left_clip.get() as u32)
-                            .min(span.size.width as u32) as usize
-                        ..pos_x
-                            + x3.floor()
-                                .saturating_sub(rr.left_clip.get() as u32)
-                                .min(span.size.width as u32)
-                                as usize],
+                    &mut line_buffer[x2
+                        .ceil()
+                        .saturating_sub((rr.left_clip.get() + extra_left_clip) as u32)
+                        .min(width as u32) as usize
+                        ..x3.floor()
+                            .saturating_sub((rr.left_clip.get() + extra_left_clip) as u32)
+                            .min(width as u32) as usize],
                     rr.border_color,
                 )
             }
             // 4. anti-aliasing for the contents (x3 .. x4)
             anti_alias(
-                x3.saturating_sub(Shifted::new(rr.left_clip.get())),
-                x4.saturating_sub(Shifted::new(rr.left_clip.get())),
+                x3.saturating_sub(Shifted::new(rr.left_clip.get() + extra_left_clip)),
+                x4.saturating_sub(Shifted::new(rr.left_clip.get() + extra_left_clip)),
                 &mut |x, cov| {
-                    if x >= span.size.width as usize {
+                    if x >= width {
                         return;
                     }
                     let col = interpolate_color(cov, rr.border_color, rr.inner_color);
-                    line_buffer[pos_x + x].blend(col);
+                    line_buffer[x].blend(col);
                 },
             );
         }
         if rr.inner_color.alpha > 0 {
             // 5. inside (x4 .. x5)
-            let begin =
-                x4.ceil().saturating_sub(rr.left_clip.get() as u32).min(span.size.width as u32);
-            let end = x5.floor().min(span.size.width as u32);
+            let begin = x4
+                .ceil()
+                .saturating_sub((rr.left_clip.get() + extra_left_clip) as u32)
+                .min(width as u32);
+            let end = x5.floor().min(width as u32);
             if begin < end {
                 TargetPixel::blend_slice(
-                    &mut line_buffer[pos_x + begin as usize..pos_x + end as usize],
+                    &mut line_buffer[begin as usize..end as usize],
                     rr.inner_color,
                 )
             }
         }
         if border > ZERO {
             // 6. border anti-aliasing: x5..x6
             anti_alias(x5, x6, &mut |x, cov| {
-                if x >= span.size.width as usize {
+                if x >= width {
                     return;
                 }
                 let col = interpolate_color(cov, rr.inner_color, rr.border_color);
-                line_buffer[pos_x + x].blend(col)
+                line_buffer[x].blend(col)
             });
             // 7. border x6 .. x7
             if ONE + x6 <= x7 {
                 TargetPixel::blend_slice(
-                    &mut line_buffer[pos_x + x6.ceil().min(span.size.width as u32) as usize
-                        ..pos_x + x7.floor().min(span.size.width as u32) as usize],
+                    &mut line_buffer[x6.ceil().min(width as u32) as usize
+                        ..x7.floor().min(width as u32) as usize],
                     rr.border_color,
                 )
             }
         }
     }
     anti_alias(x7, x8, &mut |x, cov| {
-        if x >= span.size.width as usize {
+        if x >= width {
             return;
         }
         let c = if border == ZERO { rr.inner_color } else { rr.border_color };
         let col = PremultipliedRgbaColor {
             alpha: (((c.alpha as u32) * (255 - cov) as u32) / 255) as u8,
             red: (((c.red as u32) * (255 - cov) as u32) / 255) as u8,
             green: (((c.green as u32) * (255 - cov) as u32) / 255) as u8,
             blue: (((c.blue as u32) * (255 - cov) as u32) / 255) as u8,
         };
-        line_buffer[pos_x + x].blend(col);
+        line_buffer[x].blend(col);
     });
 }
 
 // a is between 0 and 255. When 0, we get color1, when 255 we get color2
 fn interpolate_color(
     a: u32,
     color1: PremultipliedRgbaColor,
@@ -501,19 +504,17 @@
     }
 }
 
 pub(super) fn draw_gradient_line(
     rect: &PhysicalRect,
     line: PhysicalLength,
     g: &super::GradientCommand,
-    line_buffer: &mut [impl TargetPixel],
+    mut buffer: &mut [impl TargetPixel],
+    extra_left_clip: i16,
 ) {
-    let mut buffer = &mut line_buffer
-        [rect.origin.x as usize..(rect.origin.x_length() + rect.width_length()).get() as usize];
-
     let fill_col1 = g.flags & 0b010 != 0;
     let fill_col2 = g.flags & 0b100 != 0;
     let invert_slope = g.flags & 0b1 != 0;
 
     let y = (line.get() - rect.min_y() + g.top_clip.get()) as i32;
     let size_y = (rect.height() + g.top_clip.get() + g.bottom_clip.get()) as i32;
     let start = g.start as i32;
@@ -535,15 +536,16 @@
 
     let size_x = (rect.width() + g.left_clip.get() + g.right_clip.get()) as i32;
 
     let mut x = if invert_slope {
         (y * size_x * (255 - start)) / (size_y * start)
     } else {
         (size_y - y) * size_x * (255 - start) / (size_y * start)
-    } + g.left_clip.get() as i32;
+    } + g.left_clip.get() as i32
+        + extra_left_clip as i32;
 
     let len = ((255 * size_x) / start) as usize;
 
     if x < 0 {
         let l = (-x as usize).min(buffer.len());
         if invert_slope {
             if fill_col1 {
```

### Comparing `slint-1.6.0a6/internal/core/software_renderer/fixed.rs` & `slint-1.6.0a7/internal/core/software_renderer/fixed.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core/software_renderer/fonts/pixelfont.rs` & `slint-1.6.0a7/internal/core/software_renderer/fonts/pixelfont.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core/software_renderer/fonts/systemfonts.rs` & `slint-1.6.0a7/internal/core/software_renderer/fonts/systemfonts.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core/software_renderer/fonts/vectorfont.rs` & `slint-1.6.0a7/internal/core/software_renderer/fonts/vectorfont.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core/software_renderer/fonts.rs` & `slint-1.6.0a7/internal/core/software_renderer/fonts.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core/software_renderer.rs` & `slint-1.6.0a7/internal/core/software_renderer.rs`

 * *Files 10% similar despite different names*

```diff
@@ -11,48 +11,43 @@
 mod fixed;
 mod fonts;
 
 use self::fonts::GlyphRenderer;
 use crate::api::Window;
 use crate::graphics::rendering_metrics_collector::{RefreshMode, RenderingMetricsCollector};
 use crate::graphics::{BorderRadius, PixelFormat, SharedImageBuffer, SharedPixelBuffer};
-use crate::item_rendering::{
-    CachedRenderingData, ItemRenderer, RenderBorderRectangle, RenderImage,
-};
+use crate::item_rendering::{CachedRenderingData, DirtyRegion, RenderBorderRectangle, RenderImage};
 use crate::items::{ItemRc, TextOverflow};
 use crate::lengths::{
     LogicalBorderRadius, LogicalLength, LogicalPoint, LogicalRect, LogicalSize, LogicalVector,
     PhysicalPx, PointLengths, RectLengths, ScaleFactor, SizeLengths,
 };
 use crate::renderer::{Renderer, RendererSealed};
 use crate::textlayout::{AbstractFont, FontMetrics, TextParagraphLayout};
 use crate::window::{WindowAdapter, WindowInner};
 use crate::{Brush, Color, Coord, ImageInner, StaticTextures};
 use alloc::rc::{Rc, Weak};
 #[cfg(not(feature = "std"))]
 use alloc::{vec, vec::Vec};
 use core::cell::{Cell, RefCell};
 use core::pin::Pin;
-use euclid::num::Zero;
 use euclid::Length;
 use fixed::Fixed;
 #[allow(unused)]
 use num_traits::Float;
 use num_traits::NumCast;
 
 pub use draw_functions::{PremultipliedRgbaColor, Rgb565Pixel, TargetPixel};
 
 type PhysicalLength = euclid::Length<i16, PhysicalPx>;
 type PhysicalRect = euclid::Rect<i16, PhysicalPx>;
 type PhysicalSize = euclid::Size2D<i16, PhysicalPx>;
 type PhysicalPoint = euclid::Point2D<i16, PhysicalPx>;
 type PhysicalBorderRadius = BorderRadius<i16, PhysicalPx>;
 
-type DirtyRegion = PhysicalRect;
-
 /// This enum describes which parts of the buffer passed to the [`SoftwareRenderer`] may be re-used to speed up painting.
 // FIXME: #[non_exhaustive] #3023
 #[derive(PartialEq, Eq, Debug, Clone, Default, Copy)]
 pub enum RepaintBufferType {
     #[default]
     /// The full window is always redrawn. No attempt at partial rendering will be made.
     NewBuffer,
@@ -208,29 +203,141 @@
         &mut self,
         line: usize,
         range: core::ops::Range<usize>,
         render_fn: impl FnOnce(&mut [Self::TargetPixel]),
     );
 }
 
+#[cfg(not(cbindgen))]
+const PHYSICAL_REGION_MAX_SIZE: usize = DirtyRegion::MAX_COUNT;
+// cbindgen can't understand associated const correctly, so hardcode the value
+#[cfg(cbindgen)]
+pub const PHYSICAL_REGION_MAX_SIZE: usize = 3;
+const _: () = {
+    assert!(PHYSICAL_REGION_MAX_SIZE == 3);
+    assert!(DirtyRegion::MAX_COUNT == 3);
+};
+
 /// Represents a rectangular region on the screen, used for partial rendering.
 ///
 /// The region may be composed of multiple sub-regions.
 #[derive(Clone, Debug, Default)]
-pub struct PhysicalRegion(PhysicalRect);
+#[repr(C)]
+pub struct PhysicalRegion {
+    rectangles: [euclid::Box2D<i16, PhysicalPx>; PHYSICAL_REGION_MAX_SIZE],
+    count: usize,
+}
 
 impl PhysicalRegion {
+    fn iter_box(&self) -> impl Iterator<Item = euclid::Box2D<i16, PhysicalPx>> + '_ {
+        (0..self.count).map(|x| self.rectangles[x])
+    }
+
+    fn bounding_rect(&self) -> PhysicalRect {
+        if self.count == 0 {
+            return Default::default();
+        }
+        let mut r = self.rectangles[0];
+        for i in 1..self.count {
+            r = r.union(&self.rectangles[i]);
+        }
+        r.to_rect()
+    }
+
     /// Returns the size of the bounding box of this region.
     pub fn bounding_box_size(&self) -> crate::api::PhysicalSize {
-        crate::api::PhysicalSize { width: self.0.width() as _, height: self.0.height() as _ }
+        let bb = self.bounding_rect();
+        crate::api::PhysicalSize { width: bb.width() as _, height: bb.height() as _ }
     }
     /// Returns the origin of the bounding box of this region.
     pub fn bounding_box_origin(&self) -> crate::api::PhysicalPosition {
-        crate::api::PhysicalPosition { x: self.0.origin.x as _, y: self.0.origin.y as _ }
+        let bb = self.bounding_rect();
+        crate::api::PhysicalPosition { x: bb.origin.x as _, y: bb.origin.y as _ }
+    }
+
+    /// Returns an iterator over the rectangles in this region.
+    /// Each rectangle is represented by its position and its size.
+    pub fn iter(
+        &self,
+    ) -> impl Iterator<Item = (crate::api::PhysicalPosition, crate::api::PhysicalSize)> + '_ {
+        self.iter_box().map(|r| {
+            let r = r.to_rect();
+            (
+                crate::api::PhysicalPosition { x: r.origin.x as _, y: r.origin.y as _ },
+                crate::api::PhysicalSize { width: r.width() as _, height: r.height() as _ },
+            )
+        })
+    }
+}
+
+/// Computes what are the x ranges that intersects the region for specified y line.
+///
+/// This uses a mutable reference to a Vec so that the memory is re-used between calls.
+///
+/// Returns the y position until which this range is valid
+fn region_line_ranges(
+    region: &PhysicalRegion,
+    line: i16,
+    line_ranges: &mut Vec<core::ops::Range<i16>>,
+) -> Option<i16> {
+    line_ranges.clear();
+    let mut next_validity = None::<i16>;
+    for geom in region.iter_box() {
+        if geom.is_empty() {
+            continue;
+        }
+        if geom.y_range().contains(&line) {
+            match &mut next_validity {
+                Some(val) => *val = geom.max.y.min(*val),
+                None => next_validity = Some(geom.max.y),
+            }
+            let mut tmp = Some(geom.x_range());
+            line_ranges.retain_mut(|it| {
+                if let Some(r) = &mut tmp {
+                    if it.end < r.start {
+                        return true;
+                    } else if it.start <= r.start {
+                        if it.end >= r.end {
+                            tmp = None;
+                            return true;
+                        }
+                        r.start = it.start;
+                        return false;
+                    } else if it.start <= r.end {
+                        if it.end <= r.end {
+                            return false;
+                        } else {
+                            it.start = r.start;
+                            tmp = None;
+                            return true;
+                        }
+                    } else {
+                        core::mem::swap(it, r);
+                        return true;
+                    }
+                } else {
+                    return true;
+                }
+            });
+            if let Some(r) = tmp {
+                line_ranges.push(r);
+            }
+            continue;
+        } else {
+            if geom.min.y >= line {
+                match &mut next_validity {
+                    Some(val) => *val = geom.min.y.min(*val),
+                    None => next_validity = Some(geom.min.y),
+                }
+            }
+        }
     }
+    // check that current items are properly sorted
+    debug_assert!(line_ranges.windows(2).all(|x| x[0].end < x[1].start));
+    next_validity
 }
 
 /// A Renderer that do the rendering in software
 ///
 /// The renderer can remember what items needs to be redrawn from the previous iteration.
 ///
 /// There are two kind of possible rendering
@@ -238,15 +345,15 @@
 ///  2. Using [`render_by_line()`](Self::render()) to render the window line by line. This
 ///     is only useful if the device does not have enough memory to render the whole window
 ///     in one single buffer
 pub struct SoftwareRenderer {
     partial_cache: RefCell<crate::item_rendering::PartialRenderingCache>,
     repaint_buffer_type: Cell<RepaintBufferType>,
     /// This is the area which we are going to redraw in the next frame, no matter if the items are dirty or not
-    force_dirty: Cell<crate::item_rendering::DirtyRegion>,
+    force_dirty: RefCell<DirtyRegion>,
     /// Force a redraw in the next frame, no matter what's dirty. Use only as a last resort.
     force_screen_refresh: Cell<bool>,
     /// This is the area which was dirty on the previous frame.
     /// Only used if repaint_buffer_type == RepaintBufferType::SwappedBuffers
     prev_frame_dirty: Cell<DirtyRegion>,
     maybe_window_adapter: RefCell<Option<Weak<dyn crate::window::WindowAdapter>>>,
     rotation: Cell<RenderingRotation>,
@@ -309,36 +416,29 @@
     #[cfg(feature = "software-renderer-rotation")]
     pub fn rendering_rotation(&self) -> RenderingRotation {
         self.rotation.get()
     }
 
     /// Internal function to apply a dirty region depending on the dirty_tracking_policy.
     /// Returns the region to actually draw.
-    fn apply_dirty_region(
-        &self,
-        mut dirty_region: DirtyRegion,
-        screen_size: PhysicalSize,
-    ) -> DirtyRegion {
-        let screen_region = PhysicalRect { origin: euclid::point2(0, 0), size: screen_size };
+    fn apply_dirty_region(&self, dirty_region: &mut DirtyRegion, screen_size: LogicalSize) {
+        let screen_region = LogicalRect::from_size(screen_size);
 
         if self.force_screen_refresh.take() {
-            dirty_region = screen_region;
+            *dirty_region = screen_region.into();
         }
 
-        match self.repaint_buffer_type() {
-            RepaintBufferType::NewBuffer => {
-                PhysicalRect { origin: euclid::point2(0, 0), size: screen_size }
-            }
-            RepaintBufferType::ReusedBuffer => dirty_region,
+        *dirty_region = match self.repaint_buffer_type() {
+            RepaintBufferType::NewBuffer => screen_region.into(),
+            RepaintBufferType::ReusedBuffer => dirty_region.clone(),
             RepaintBufferType::SwappedBuffers => {
-                dirty_region.union(&self.prev_frame_dirty.replace(dirty_region))
+                dirty_region.union(&self.prev_frame_dirty.replace(dirty_region.clone()))
             }
         }
-        .intersection(&screen_region)
-        .unwrap_or_default()
+        .intersection(screen_region)
     }
 
     /// Render the window to the given frame buffer.
     ///
     /// The renderer uses a cache internally and will only render the part of the window
     /// which are dirty. The `extra_draw_region` is an extra regin which will also
     /// be rendered. (eg: the previous dirty region in case of double buffering)
@@ -383,54 +483,66 @@
             },
             "buffer of size {} with stride {pixel_stride} is too small to handle a window of size {size:?}", buffer.len()
         );
         let buffer_renderer = SceneBuilder::new(
             size,
             factor,
             window_inner,
-            RenderToBuffer { buffer, stride: pixel_stride },
+            RenderToBuffer {
+                buffer,
+                stride: pixel_stride,
+                dirty_range_cache: vec![],
+                dirty_region: Default::default(),
+            },
             rotation,
         );
         let mut renderer = crate::item_rendering::PartialRenderer::new(
             &self.partial_cache,
             self.force_dirty.take(),
             buffer_renderer,
         );
 
         window_inner
             .draw_contents(|components| {
+                let logical_size = (size.cast() / factor).cast();
                 for (component, origin) in components {
-                    renderer.compute_dirty_regions(component, *origin);
+                    renderer.compute_dirty_regions(component, *origin, logical_size);
                 }
-
-                let dirty_region = (renderer.dirty_region.to_rect().cast() * factor)
-                    .round_out()
-                    .intersection(&euclid::rect(0., 0., i16::MAX as f32, i16::MAX as f32))
-                    .unwrap_or_default()
-                    .cast();
-
-                let to_draw = self.apply_dirty_region(dirty_region, size);
-
-                renderer.combine_clip(
-                    (to_draw.cast() / factor).cast(),
-                    LogicalBorderRadius::zero(),
-                    LogicalLength::zero(),
-                );
+                self.apply_dirty_region(&mut renderer.dirty_region, logical_size);
+                let rotation = RotationInfo { orientation: rotation, screen_size: size };
+                let mut i = renderer.dirty_region.iter().map(|r| {
+                    (r.cast() * factor).to_rect().round_out().cast().transformed(rotation)
+                });
+                let dirty_region = PhysicalRegion {
+                    rectangles: core::array::from_fn(|_| i.next().unwrap_or_default().to_box2d()),
+                    count: renderer.dirty_region.iter().count(),
+                };
+                drop(i);
 
                 let mut bg = TargetPixel::background();
                 // TODO: gradient background
                 TargetPixel::blend(&mut bg, background.color().into());
-                let to_draw_tr = to_draw.transformed(renderer.actual_renderer.rotation);
-                for line in to_draw_tr.min_y()..to_draw_tr.max_y() {
-                    let begin = line as usize * pixel_stride + to_draw_tr.origin.x as usize;
-                    renderer.actual_renderer.processor.buffer[begin..]
-                        [..to_draw_tr.width() as usize]
-                        .fill(bg);
+                let mut line = 0;
+                while let Some(next) = region_line_ranges(
+                    &dirty_region,
+                    line,
+                    &mut renderer.actual_renderer.processor.dirty_range_cache,
+                ) {
+                    for l in line..next {
+                        for r in &renderer.actual_renderer.processor.dirty_range_cache {
+                            renderer.actual_renderer.processor.buffer[l as usize * pixel_stride..]
+                                [r.start as usize..r.end as usize]
+                                .fill(bg);
+                        }
+                    }
+                    line = next;
                 }
 
+                renderer.actual_renderer.processor.dirty_region = dirty_region.clone();
+
                 for (component, origin) in components {
                     crate::item_rendering::render_component_items(
                         component,
                         &mut renderer,
                         *origin,
                     );
                 }
@@ -438,15 +550,15 @@
                 if let Some(metrics) = &self.rendering_metrics_collector {
                     metrics.measure_frame_rendered(&mut renderer);
                     if metrics.refresh_mode() == RefreshMode::FullSpeed {
                         self.force_screen_refresh.set(true);
                     }
                 }
 
-                PhysicalRegion(to_draw_tr)
+                dirty_region
             })
             .unwrap_or_default()
     }
 
     /// Render the window, line by line, into the line buffer provided by the [`LineBufferProvider`].
     ///
     /// The renderer uses a cache internally and will only render the part of the window
@@ -499,15 +611,15 @@
                 window_inner,
                 window_item.background(),
                 size.cast(),
                 self,
                 line_buffer,
             )
         } else {
-            PhysicalRegion(Default::default())
+            PhysicalRegion { ..Default::default() }
         }
     }
 }
 
 #[doc(hidden)]
 impl RendererSealed for SoftwareRenderer {
     fn text_size(
@@ -656,15 +768,15 @@
         // We don't have a way to determine the screen region of the delete items, what's in the cache is relative. So
         // as a last resort, refresh everything.
         self.force_screen_refresh.set(true);
         Ok(())
     }
 
     fn mark_dirty_region(&self, region: crate::item_rendering::DirtyRegion) {
-        self.force_dirty.set(self.force_dirty.get().union(&region))
+        self.force_dirty.replace_with(|r| r.union(&region));
     }
 
     fn register_bitmap_font(&self, font_data: &'static crate::graphics::BitmapFont) {
         fonts::register_bitmap_font(font_data);
     }
 
     #[cfg(all(feature = "software-renderer-systemfonts", not(target_arch = "wasm32")))]
@@ -696,110 +808,110 @@
 fn render_window_frame_by_line(
     window: &WindowInner,
     background: Brush,
     size: PhysicalSize,
     renderer: &SoftwareRenderer,
     mut line_buffer: impl LineBufferProvider,
 ) -> PhysicalRegion {
-    let rotation = RotationInfo { orientation: renderer.rotation.get(), screen_size: size };
     let mut scene = prepare_scene(window, size, renderer);
 
-    let dirty_region = scene.dirty_region;
-    let to_draw_tr = dirty_region.transformed(rotation);
-
-    scene.current_line = to_draw_tr.origin.y_length();
+    let to_draw_tr = scene.dirty_region.bounding_rect();
 
     let mut background_color = TargetPixel::background();
     // FIXME gradient
     TargetPixel::blend(&mut background_color, background.color().into());
 
     while scene.current_line < to_draw_tr.origin.y_length() + to_draw_tr.size.height_length() {
-        line_buffer.process_line(
-            scene.current_line.get() as usize,
-            to_draw_tr.min_x() as usize..to_draw_tr.max_x() as usize,
-            |line_buffer| {
-                let offset = to_draw_tr.min_x() as usize;
-
-                line_buffer.fill(background_color);
-                for span in scene.items[0..scene.current_items_index].iter().rev() {
-                    debug_assert!(scene.current_line >= span.pos.y_length());
-                    debug_assert!(
-                        scene.current_line < span.pos.y_length() + span.size.height_length(),
-                    );
-                    match span.command {
-                        SceneCommand::Rectangle { color } => {
-                            TargetPixel::blend_slice(
-                                &mut line_buffer[span.pos.x as usize - offset
-                                    ..(span.pos.x_length() + span.size.width_length()).get()
-                                        as usize
-                                        - offset],
-                                color,
-                            );
-                        }
-                        SceneCommand::Texture { texture_index } => {
-                            let texture = &scene.vectors.textures[texture_index as usize];
-                            draw_functions::draw_texture_line(
-                                &PhysicalRect {
-                                    origin: span.pos - euclid::vec2(offset as i16, 0),
-                                    size: span.size,
-                                },
-                                scene.current_line,
-                                texture,
-                                line_buffer,
-                            );
-                        }
-                        SceneCommand::SharedBuffer { shared_buffer_index } => {
-                            let texture = scene.vectors.shared_buffers
-                                [shared_buffer_index as usize]
-                                .as_texture();
-                            draw_functions::draw_texture_line(
-                                &PhysicalRect {
-                                    origin: span.pos - euclid::vec2(offset as i16, 0),
-                                    size: span.size,
-                                },
-                                scene.current_line,
-                                &texture,
-                                line_buffer,
-                            );
+        for r in &scene.current_line_ranges {
+            line_buffer.process_line(
+                scene.current_line.get() as usize,
+                r.start as usize..r.end as usize,
+                |line_buffer| {
+                    let offset = r.start;
+
+                    line_buffer.fill(background_color);
+                    for span in scene.items[0..scene.current_items_index].iter().rev() {
+                        debug_assert!(scene.current_line >= span.pos.y_length());
+                        debug_assert!(
+                            scene.current_line < span.pos.y_length() + span.size.height_length(),
+                        );
+                        if span.pos.x >= r.end {
+                            continue;
                         }
-                        SceneCommand::RoundedRectangle { rectangle_index } => {
-                            let rr = &scene.vectors.rounded_rectangles[rectangle_index as usize];
-                            draw_functions::draw_rounded_rectangle_line(
-                                &PhysicalRect {
-                                    origin: span.pos - euclid::vec2(offset as i16, 0),
-                                    size: span.size,
-                                },
-                                scene.current_line,
-                                rr,
-                                line_buffer,
-                            );
+                        let begin = r.start.max(span.pos.x);
+                        let end = r.end.min(span.pos.x + span.size.width);
+                        if begin >= end {
+                            continue;
                         }
-                        SceneCommand::Gradient { gradient_index } => {
-                            let g = &scene.vectors.gradients[gradient_index as usize];
 
-                            draw_functions::draw_gradient_line(
-                                &PhysicalRect {
-                                    origin: span.pos - euclid::vec2(offset as i16, 0),
-                                    size: span.size,
-                                },
-                                scene.current_line,
-                                g,
-                                line_buffer,
-                            );
+                        let extra_left_clip = begin - span.pos.x;
+                        let extra_right_clip = span.pos.x + span.size.width - end;
+                        let range_buffer =
+                            &mut line_buffer[(begin - offset) as usize..(end - offset) as usize];
+
+                        match span.command {
+                            SceneCommand::Rectangle { color } => {
+                                TargetPixel::blend_slice(range_buffer, color);
+                            }
+                            SceneCommand::Texture { texture_index } => {
+                                let texture = &scene.vectors.textures[texture_index as usize];
+                                draw_functions::draw_texture_line(
+                                    &PhysicalRect { origin: span.pos, size: span.size },
+                                    scene.current_line,
+                                    texture,
+                                    range_buffer,
+                                    extra_left_clip,
+                                );
+                            }
+                            SceneCommand::SharedBuffer { shared_buffer_index } => {
+                                let texture = scene.vectors.shared_buffers
+                                    [shared_buffer_index as usize]
+                                    .as_texture();
+                                draw_functions::draw_texture_line(
+                                    &PhysicalRect { origin: span.pos, size: span.size },
+                                    scene.current_line,
+                                    &texture,
+                                    range_buffer,
+                                    extra_left_clip,
+                                );
+                            }
+                            SceneCommand::RoundedRectangle { rectangle_index } => {
+                                let rr =
+                                    &scene.vectors.rounded_rectangles[rectangle_index as usize];
+                                draw_functions::draw_rounded_rectangle_line(
+                                    &PhysicalRect { origin: span.pos, size: span.size },
+                                    scene.current_line,
+                                    rr,
+                                    range_buffer,
+                                    extra_left_clip,
+                                    extra_right_clip,
+                                );
+                            }
+                            SceneCommand::Gradient { gradient_index } => {
+                                let g = &scene.vectors.gradients[gradient_index as usize];
+
+                                draw_functions::draw_gradient_line(
+                                    &PhysicalRect { origin: span.pos, size: span.size },
+                                    scene.current_line,
+                                    g,
+                                    range_buffer,
+                                    extra_left_clip,
+                                );
+                            }
                         }
                     }
-                }
-            },
-        );
+                },
+            );
+        }
 
         if scene.current_line < to_draw_tr.origin.y_length() + to_draw_tr.size.height_length() {
             scene.next_line();
         }
     }
-    PhysicalRegion(to_draw_tr)
+    scene.dirty_region
 }
 
 #[derive(Default)]
 struct SceneVectors {
     textures: Vec<SceneTexture<'static>>,
     rounded_rectangles: Vec<RoundedRectangle>,
     shared_buffers: Vec<SharedBufferCommand>,
@@ -818,42 +930,53 @@
     items: Vec<SceneItem>,
 
     vectors: SceneVectors,
 
     future_items_index: usize,
     current_items_index: usize,
 
-    dirty_region: DirtyRegion,
+    dirty_region: PhysicalRegion,
+
+    current_line_ranges: Vec<core::ops::Range<i16>>,
+    range_valid_until_line: PhysicalLength,
 }
 
 impl Scene {
     pub fn new(
         mut items: Vec<SceneItem>,
         vectors: SceneVectors,
-        dirty_region: DirtyRegion,
+        dirty_region: PhysicalRegion,
     ) -> Self {
-        let current_line = dirty_region.origin.y_length();
+        let current_line =
+            dirty_region.iter_box().map(|x| x.min.y_length()).min().unwrap_or_default();
         items.retain(|i| i.pos.y_length() + i.size.height_length() > current_line);
         items.sort_unstable_by(compare_scene_item);
         let current_items_index = items.partition_point(|i| i.pos.y_length() <= current_line);
         items[..current_items_index].sort_unstable_by(|a, b| b.z.cmp(&a.z));
-        Self {
+        let mut r = Self {
             items,
             current_line,
             current_items_index,
             future_items_index: current_items_index,
             vectors,
             dirty_region,
-        }
+            current_line_ranges: Default::default(),
+            range_valid_until_line: Default::default(),
+        };
+        r.recompute_ranges();
+        debug_assert_eq!(r.current_line, r.dirty_region.bounding_rect().origin.y_length());
+        r
     }
 
     /// Updates `current_items_index` and `future_items_index` to match the invariant
     pub fn next_line(&mut self) {
         self.current_line += PhysicalLength::new(1);
 
+        let skipped = self.current_line >= self.range_valid_until_line && self.recompute_ranges();
+
         // The items array is split in part:
         // 1. [0..i] are the items that have already been processed, that are on this line
         // 2. [j..current_items_index] are the items from the previous line that might still be
         //   valid on this line
         // 3. [tmp1, tmp2] is a buffer where we swap items so we can make room for the items in [0..i]
         // 4. [future_items_index..] are the items which might get processed now
         // 5. [current_items_index..tmp1], [tmp2..future_items_index] and [i..j] is garbage
@@ -861,14 +984,41 @@
         // At each step, we selecting the item with the higher z from the list 2 or 3 or 4 and take it from
         // that list. Then we add it to the list [0..i] if it needs more processing. If needed,
         // we move the first  item from list  2. to list 3. to make some room
 
         let (mut i, mut j, mut tmp1, mut tmp2) =
             (0, 0, self.current_items_index, self.current_items_index);
 
+        if skipped {
+            // Merge sort doesn't work in that case.
+            while j < self.current_items_index {
+                let item = self.items[j];
+                if item.pos.y_length() + item.size.height_length() > self.current_line {
+                    self.items[i] = item;
+                    i += 1;
+                }
+                j += 1;
+            }
+            while self.future_items_index < self.items.len() {
+                let item = self.items[self.future_items_index];
+                if item.pos.y_length() > self.current_line {
+                    break;
+                }
+                self.future_items_index += 1;
+                if item.pos.y_length() + item.size.height_length() < self.current_line {
+                    continue;
+                }
+                self.items[i] = item;
+                i += 1;
+            }
+            self.items[0..i].sort_unstable_by(|a, b| b.z.cmp(&a.z));
+            self.current_items_index = i;
+            return;
+        }
+
         'outer: loop {
             let future_next_z = self
                 .items
                 .get(self.future_items_index)
                 .filter(|i| i.pos.y_length() <= self.current_line)
                 .map(|i| i.z);
             let item = loop {
@@ -933,28 +1083,53 @@
                 self.items[i] = item;
                 i += 1;
                 while self.future_items_index < self.items.len() {
                     let item = self.items[self.future_items_index];
                     if item.pos.y_length() > self.current_line {
                         break;
                     }
+                    self.future_items_index += 1;
                     self.items[i] = item;
                     i += 1;
-                    self.future_items_index += 1;
                 }
                 self.items[sort_begin..i].sort_unstable_by(|a, b| b.z.cmp(&a.z));
                 break;
             }
             self.items[i] = item;
             i += 1;
         }
         self.current_items_index = i;
         // check that current items are properly sorted
         debug_assert!(self.items[0..self.current_items_index].windows(2).all(|x| x[0].z >= x[1].z));
     }
+
+    // return true if lines were skipped
+    fn recompute_ranges(&mut self) -> bool {
+        let validity = region_line_ranges(
+            &self.dirty_region,
+            self.current_line.get(),
+            &mut self.current_line_ranges,
+        );
+        if self.current_line_ranges.is_empty() {
+            if let Some(next) = validity {
+                self.current_line = Length::new(next);
+                self.range_valid_until_line = Length::new(
+                    region_line_ranges(
+                        &self.dirty_region,
+                        self.current_line.get(),
+                        &mut self.current_line_ranges,
+                    )
+                    .unwrap_or_default(),
+                );
+                return true;
+            }
+        }
+        self.range_valid_until_line = Length::new(validity.unwrap_or_default());
+        false
+    }
 }
 
 #[derive(Clone, Copy, Debug)]
 struct SceneItem {
     pos: PhysicalPoint,
     size: PhysicalSize,
     // this is the order of the item from which it is in the item tree
@@ -1161,108 +1336,175 @@
     );
     let mut renderer = crate::item_rendering::PartialRenderer::new(
         &software_renderer.partial_cache,
         software_renderer.force_dirty.take(),
         prepare_scene,
     );
 
-    let mut dirty_region = PhysicalRect::default();
+    let mut dirty_region = PhysicalRegion::default();
     window.draw_contents(|components| {
+        let logical_size = (size.cast() / factor).cast();
         for (component, origin) in components {
-            renderer.compute_dirty_regions(component, *origin);
+            renderer.compute_dirty_regions(component, *origin, logical_size);
         }
 
-        dirty_region = (renderer.dirty_region.to_rect().cast() * factor).round_out().cast();
-        dirty_region = software_renderer.apply_dirty_region(dirty_region, size);
+        software_renderer.apply_dirty_region(&mut renderer.dirty_region, logical_size);
+        let rotation =
+            RotationInfo { orientation: software_renderer.rotation.get(), screen_size: size };
+        let mut i = renderer
+            .dirty_region
+            .iter()
+            .map(|r| (r.cast() * factor).to_rect().round_out().cast().transformed(rotation));
+        dirty_region = PhysicalRegion {
+            rectangles: core::array::from_fn(|_| i.next().unwrap_or_default().to_box2d()),
+            count: renderer.dirty_region.iter().count(),
+        };
+        drop(i);
 
-        renderer.combine_clip(
-            (dirty_region.cast() / factor).cast(),
-            LogicalBorderRadius::zero(),
-            LogicalLength::zero(),
-        );
         for (component, origin) in components {
             crate::item_rendering::render_component_items(component, &mut renderer, *origin);
         }
     });
 
     if let Some(metrics) = &software_renderer.rendering_metrics_collector {
         metrics.measure_frame_rendered(&mut renderer);
         if metrics.refresh_mode() == RefreshMode::FullSpeed {
             software_renderer.force_screen_refresh.set(true);
         }
     }
 
     let prepare_scene = renderer.into_inner();
 
+    /* // visualize dirty regions
+    let mut prepare_scene = prepare_scene;
+    for rect in dirty_region.iter() {
+        prepare_scene.processor.process_rounded_rectangle(
+            rect.to_rect(),
+            RoundedRectangle {
+                radius: BorderRadius::default(),
+                width: Length::new(1),
+                border_color: Color::from_argb_u8(128, 255, 0, 0).into(),
+                inner_color: PremultipliedRgbaColor::default(),
+                left_clip: Length::default(),
+                right_clip: Length::default(),
+                top_clip: Length::default(),
+                bottom_clip: Length::default(),
+            },
+        )
+    } // */
+
     Scene::new(prepare_scene.processor.items, prepare_scene.processor.vectors, dirty_region)
 }
 
 trait ProcessScene {
     fn process_texture(&mut self, geometry: PhysicalRect, texture: SceneTexture<'static>);
     fn process_rectangle(&mut self, geometry: PhysicalRect, color: PremultipliedRgbaColor);
     fn process_rounded_rectangle(&mut self, geometry: PhysicalRect, data: RoundedRectangle);
     fn process_shared_image_buffer(&mut self, geometry: PhysicalRect, buffer: SharedBufferCommand);
     fn process_gradient(&mut self, geometry: PhysicalRect, gradient: GradientCommand);
 }
 
 struct RenderToBuffer<'a, TargetPixel> {
     buffer: &'a mut [TargetPixel],
     stride: usize,
+    dirty_range_cache: Vec<core::ops::Range<i16>>,
+    dirty_region: PhysicalRegion,
 }
 
 impl<'a, T: TargetPixel> RenderToBuffer<'a, T> {
+    fn foreach_ranges(
+        &mut self,
+        geometry: &PhysicalRect,
+        mut f: impl FnMut(i16, &mut [T], i16, i16),
+    ) {
+        let mut line = geometry.min_y();
+        while let Some(mut next) =
+            region_line_ranges(&self.dirty_region, line, &mut self.dirty_range_cache)
+        {
+            next = next.min(geometry.max_y());
+            for r in &self.dirty_range_cache {
+                if geometry.origin.x >= r.end {
+                    continue;
+                }
+                let begin = r.start.max(geometry.origin.x);
+                let end = r.end.min(geometry.origin.x + geometry.size.width);
+                if begin >= end {
+                    continue;
+                }
+                let extra_left_clip = begin - geometry.origin.x;
+                let extra_right_clip = geometry.origin.x + geometry.size.width - end;
+
+                for l in line..next {
+                    f(
+                        l,
+                        &mut self.buffer[l as usize * self.stride..][begin as usize..end as usize],
+                        extra_left_clip,
+                        extra_right_clip,
+                    );
+                }
+            }
+            if next == geometry.max_y() {
+                break;
+            }
+            line = next;
+        }
+    }
+
     fn process_texture_impl(&mut self, geometry: PhysicalRect, texture: SceneTexture<'_>) {
-        for line in geometry.min_y()..geometry.max_y() {
+        self.foreach_ranges(&geometry, |line, buffer, extra_left_clip, _extra_right_clip| {
             draw_functions::draw_texture_line(
                 &geometry,
                 PhysicalLength::new(line),
                 &texture,
-                &mut self.buffer[line as usize * self.stride..],
+                buffer,
+                extra_left_clip,
             );
-        }
+        });
     }
 }
 
 impl<'a, T: TargetPixel> ProcessScene for RenderToBuffer<'a, T> {
     fn process_texture(&mut self, geometry: PhysicalRect, texture: SceneTexture<'static>) {
         self.process_texture_impl(geometry, texture)
     }
 
     fn process_shared_image_buffer(&mut self, geometry: PhysicalRect, buffer: SharedBufferCommand) {
         let texture = buffer.as_texture();
         self.process_texture_impl(geometry, texture);
     }
 
     fn process_rectangle(&mut self, geometry: PhysicalRect, color: PremultipliedRgbaColor) {
-        for line in geometry.min_y()..geometry.max_y() {
-            let begin = line as usize * self.stride + geometry.origin.x as usize;
-            TargetPixel::blend_slice(&mut self.buffer[begin..][..geometry.width() as usize], color);
-        }
+        self.foreach_ranges(&geometry, |_line, buffer, _extra_left_clip, _extra_right_clip| {
+            TargetPixel::blend_slice(buffer, color);
+        });
     }
 
     fn process_rounded_rectangle(&mut self, geometry: PhysicalRect, rr: RoundedRectangle) {
-        for line in geometry.min_y()..geometry.max_y() {
+        self.foreach_ranges(&geometry, |line, buffer, extra_left_clip, extra_right_clip| {
             draw_functions::draw_rounded_rectangle_line(
                 &geometry,
                 PhysicalLength::new(line),
                 &rr,
-                &mut self.buffer[line as usize * self.stride..],
+                buffer,
+                extra_left_clip,
+                extra_right_clip,
             );
-        }
+        });
     }
 
     fn process_gradient(&mut self, geometry: PhysicalRect, g: GradientCommand) {
-        for line in geometry.min_y()..geometry.max_y() {
+        self.foreach_ranges(&geometry, |line, buffer, extra_left_clip, _extra_right_clip| {
             draw_functions::draw_gradient_line(
                 &geometry,
                 PhysicalLength::new(line),
                 &g,
-                &mut self.buffer[line as usize * self.stride..],
+                buffer,
+                extra_left_clip,
             );
-        }
+        });
     }
 }
 
 #[derive(Default)]
 struct PrepareScene {
     items: Vec<SceneItem>,
     vectors: SceneVectors,
@@ -2206,14 +2448,18 @@
     }
 
     fn translate(&mut self, distance: LogicalVector) {
         self.current_state.offset += distance;
         self.current_state.clip = self.current_state.clip.translate(-distance)
     }
 
+    fn translation(&self) -> LogicalVector {
+        self.current_state.offset.to_vector()
+    }
+
     fn rotate(&mut self, _angle_in_degrees: f32) {
         todo!()
     }
 
     fn apply_opacity(&mut self, opacity: f32) {
         self.current_state.alpha *= opacity;
     }
```

### Comparing `slint-1.6.0a6/internal/core/string.rs` & `slint-1.6.0a7/internal/core/string.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core/tests.rs` & `slint-1.6.0a7/internal/core/tests.rs`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     let tick = crate::animations::CURRENT_ANIMATION_DRIVER.with(|driver| {
         let mut tick = driver.current_tick();
         tick += core::time::Duration::from_millis(time_in_ms);
         driver.update_animations(tick);
         tick
     });
     crate::timers::TimerList::maybe_activate_timers(tick);
+    crate::properties::ChangeTracker::run_change_handlers();
 }
 
 /// Return the current mocked time.
 #[no_mangle]
 pub extern "C" fn slint_get_mocked_time() -> u64 {
     crate::animations::CURRENT_ANIMATION_DRIVER.with(|driver| driver.current_tick()).as_millis()
 }
```

### Comparing `slint-1.6.0a6/internal/core/textlayout/fragments.rs` & `slint-1.6.0a7/internal/core/textlayout/fragments.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core/textlayout/glyphclusters.rs` & `slint-1.6.0a7/internal/core/textlayout/glyphclusters.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core/textlayout/linebreak_simple.rs` & `slint-1.6.0a7/internal/core/textlayout/linebreak_simple.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core/textlayout/linebreak_unicode.rs` & `slint-1.6.0a7/internal/core/textlayout/linebreak_unicode.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core/textlayout/linebreaker.rs` & `slint-1.6.0a7/internal/core/textlayout/linebreaker.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core/textlayout/shaping.rs` & `slint-1.6.0a7/internal/core/textlayout/shaping.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core/textlayout.rs` & `slint-1.6.0a7/internal/core/textlayout.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core/timers.rs` & `slint-1.6.0a7/internal/core/timers.rs`

 * *Files 0% similar despite different names*

```diff
@@ -48,26 +48,28 @@
 /// around for as long as you want the timer to keep firing.
 ///
 /// The timer can only be used in the thread that runs the Slint event loop.
 /// They will not fire if used in another thread.
 ///
 /// ## Example
 /// ```rust,no_run
-/// # i_slint_backend_testing::init();
+/// # i_slint_backend_testing::init_no_event_loop();
 /// use slint::{Timer, TimerMode};
 /// let timer = Timer::default();
 /// timer.start(TimerMode::Repeated, std::time::Duration::from_millis(200), move || {
 ///    println!("This will be printed every 200ms.");
 /// });
 /// // ... more initialization ...
 /// slint::run_event_loop();
 /// ```
 #[derive(Default)]
 pub struct Timer {
     id: Cell<Option<NonZeroUsize>>,
+    /// The timer cannot be moved between treads
+    _phantom: core::marker::PhantomData<*mut ()>,
 }
 
 impl Timer {
     /// Starts the timer with the given mode and interval, in order for the callback to called when the
     /// timer fires. If the timer has been started previously and not fired yet, then it will be restarted.
     ///
     /// Arguments:
@@ -98,15 +100,15 @@
     ///
     /// Arguments:
     /// * `duration`: The duration from now until when the timer should fire.
     /// * `callback`: The function to call when the time has been reached or exceeded.
     ///
     /// ## Example
     /// ```rust
-    /// # i_slint_backend_testing::init();
+    /// # i_slint_backend_testing::init_no_event_loop();
     /// use slint::Timer;
     /// Timer::single_shot(std::time::Duration::from_millis(200), move || {
     ///    println!("This will be printed after 200ms.");
     /// });
     /// ```
     pub fn single_shot(duration: core::time::Duration, callback: impl FnOnce() + 'static) {
         CURRENT_TIMERS.with(|timers| {
@@ -492,56 +494,56 @@
 
     /// Stop a timer and free its raw data
     #[no_mangle]
     pub extern "C" fn slint_timer_destroy(id: usize) {
         if id == 0 {
             return;
         }
-        let timer = Timer { id: Cell::new(NonZeroUsize::new(id)) };
+        let timer = Timer { id: Cell::new(NonZeroUsize::new(id)), _phantom: Default::default() };
         drop(timer);
     }
 
     /// Stop a timer
     #[no_mangle]
     pub extern "C" fn slint_timer_stop(id: usize) {
         if id == 0 {
             return;
         }
-        let timer = Timer { id: Cell::new(NonZeroUsize::new(id)) };
+        let timer = Timer { id: Cell::new(NonZeroUsize::new(id)), _phantom: Default::default() };
         timer.stop();
         timer.id.take(); // Make sure that dropping the Timer doesn't unregister it. C++ will call destroy() in the destructor.
     }
 
     /// Restart a repeated timer
     #[no_mangle]
     pub extern "C" fn slint_timer_restart(id: usize) {
         if id == 0 {
             return;
         }
-        let timer = Timer { id: Cell::new(NonZeroUsize::new(id)) };
+        let timer = Timer { id: Cell::new(NonZeroUsize::new(id)), _phantom: Default::default() };
         timer.restart();
         timer.id.take(); // Make sure that dropping the Timer doesn't unregister it. C++ will call destroy() in the destructor.
     }
 
     /// Returns true if the timer is running; false otherwise.
     #[no_mangle]
     pub extern "C" fn slint_timer_running(id: usize) -> bool {
         if id == 0 {
             return false;
         }
-        let timer = Timer { id: Cell::new(NonZeroUsize::new(id)) };
+        let timer = Timer { id: Cell::new(NonZeroUsize::new(id)), _phantom: Default::default() };
         let running = timer.running();
         timer.id.take(); // Make sure that dropping the Timer doesn't unregister it. C++ will call destroy() in the destructor.
         running
     }
 }
 
 /**
 ```rust
-i_slint_backend_testing::init();
+i_slint_backend_testing::init_no_event_loop();
 use slint::{Timer, TimerMode};
 use std::{rc::Rc, cell::RefCell, time::Duration};
 #[derive(Default)]
 struct SharedState {
     timer_200: Timer,
     timer_200_called: usize,
     timer_500: Timer,
@@ -715,15 +717,15 @@
 
 /**
  * Test that deleting an active timer from a timer event works.
 ```rust
 // There is a 200 ms timer that increase variable1
 // after 500ms, that timer is destroyed by a single shot timer,
 // and a new new timer  increase variable2
-i_slint_backend_testing::init();
+i_slint_backend_testing::init_no_event_loop();
 use slint::{Timer, TimerMode};
 use std::{rc::Rc, cell::RefCell, time::Duration};
 #[derive(Default)]
 struct SharedState {
     repeated_timer: Timer,
     variable1: usize,
     variable2: usize,
@@ -773,15 +775,15 @@
 #[cfg(doctest)]
 const _BUG3029: () = ();
 
 /**
  * Test that starting a singleshot timer works
 ```rust
 // There is a 200 ms singleshot timer that increase variable1
-i_slint_backend_testing::init();
+i_slint_backend_testing::init_no_event_loop();
 use slint::{Timer, TimerMode};
 use std::{rc::Rc, cell::RefCell, time::Duration};
 #[derive(Default)]
 struct SharedState {
     variable1: usize,
 }
 let state = Rc::new(RefCell::new(SharedState::default()));
```

### Comparing `slint-1.6.0a6/internal/core/translations.rs` & `slint-1.6.0a7/internal/core/translations.rs`

 * *Files 11% similar despite different names*

```diff
@@ -188,14 +188,18 @@
     use core::fmt::Write;
     write!(output, "{}", formatter::format(&translated, &WithPlural(arguments, n))).unwrap();
     output
 }
 
 #[cfg(all(target_family = "unix", feature = "gettext-rs"))]
 fn translate_gettext(string: &str, ctx: &str, domain: &str, n: i32, plural: &str) -> String {
+    crate::context::GLOBAL_CONTEXT.with(|ctx| {
+        let Some(ctx) = ctx.get() else { return };
+        ctx.0.translations_dirty.as_ref().get();
+    });
     fn mangle_context(ctx: &str, s: &str) -> String {
         format!("{}\u{4}{}", ctx, s)
     }
     fn demangle_context(r: String) -> String {
         if let Some(x) = r.split('\u{4}').last() {
             return x.to_owned();
         }
@@ -216,43 +220,55 @@
             n as u32,
         ))
     } else {
         gettextrs::dngettext(domain, string, plural, n as u32)
     }
 }
 
+pub fn mark_all_translations_dirty() {
+    crate::context::GLOBAL_CONTEXT.with(|ctx| {
+        let Some(ctx) = ctx.get() else { return };
+        ctx.0.translations_dirty.mark_dirty();
+    })
+}
+
 #[cfg(feature = "gettext-rs")]
 /// Initialize the translation by calling the [`bindtextdomain`](https://man7.org/linux/man-pages/man3/bindtextdomain.3.html) function from gettext
 pub fn gettext_bindtextdomain(_domain: &str, _dirname: std::path::PathBuf) -> std::io::Result<()> {
     #[cfg(target_family = "unix")]
     {
         gettextrs::bindtextdomain(_domain, _dirname)?;
         static START: std::sync::Once = std::sync::Once::new();
         START.call_once(|| {
             gettextrs::setlocale(gettextrs::LocaleCategory::LcAll, "");
         });
+        mark_all_translations_dirty();
     }
     Ok(())
 }
 
 #[cfg(feature = "ffi")]
 mod ffi {
     #![allow(unsafe_code)]
     use super::*;
     use crate::slice::Slice;
 
+    /// Perform the translation and formatting.
     #[no_mangle]
-    /// Returns a nul-terminated pointer for this string.
-    /// The returned value is owned by the string, and should not be used after any
-    /// mutable function have been called on the string, and must not be freed.
     pub extern "C" fn slint_translate(
         to_translate: &mut SharedString,
         context: &SharedString,
         domain: &SharedString,
         arguments: Slice<SharedString>,
         n: i32,
         plural: &SharedString,
     ) {
         *to_translate =
             translate(to_translate.as_str(), &context, &domain, arguments.as_slice(), n, &plural)
     }
+
+    /// Mark all translated string as dirty to perform re-translation in case the language change
+    #[no_mangle]
+    pub extern "C" fn slint_translations_mark_dirty() {
+        mark_all_translations_dirty();
+    }
 }
```

### Comparing `slint-1.6.0a6/internal/core/unsafe_single_threaded.rs` & `slint-1.6.0a7/internal/core/unsafe_single_threaded.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core/window.rs` & `slint-1.6.0a7/internal/core/window.rs`

 * *Files 1% similar despite different names*

```diff
@@ -320,30 +320,30 @@
 }
 
 struct WindowPropertiesTracker {
     window_adapter_weak: Weak<dyn WindowAdapter>,
 }
 
 impl crate::properties::PropertyDirtyHandler for WindowPropertiesTracker {
-    fn notify(&self) {
+    fn notify(self: Pin<&Self>) {
         let win = self.window_adapter_weak.clone();
         crate::timers::Timer::single_shot(Default::default(), move || {
             if let Some(window_adapter) = win.upgrade() {
                 WindowInner::from_pub(window_adapter.window()).update_window_properties();
             };
         })
     }
 }
 
 struct WindowRedrawTracker {
     window_adapter_weak: Weak<dyn WindowAdapter>,
 }
 
 impl crate::properties::PropertyDirtyHandler for WindowRedrawTracker {
-    fn notify(&self) {
+    fn notify(self: Pin<&Self>) {
         if let Some(window_adapter) = self.window_adapter_weak.upgrade() {
             window_adapter.request_redraw();
         };
     }
 }
 
 /// This enum describes the different ways a popup can be rendered by the back-end.
@@ -614,14 +614,16 @@
 
         if close_popup_on_click
             && ((mouse_inside_popup && released_event && self.had_popup_on_press.get())
                 || (!mouse_inside_popup && pressed_event))
         {
             self.close_popup();
         }
+
+        crate::properties::ChangeTracker::run_change_handlers();
     }
 
     /// Called by the input code's internal timer to send an event that was delayed
     pub(crate) fn process_delayed_event(&self) {
         self.mouse_input_state.set(crate::input::process_delayed_event(
             &self.window_adapter(),
             self.mouse_input_state.take(),
@@ -653,14 +655,15 @@
                 self.take_focus_item();
             } else if focus_item.borrow().as_ref().key_event(
                 &event,
                 &self.window_adapter(),
                 &focus_item,
             ) == crate::input::KeyEventResult::EventAccepted
             {
+                crate::properties::ChangeTracker::run_change_handlers();
                 return;
             }
             item = focus_item.parent_item();
         }
 
         // Make Tab/Backtab handle keyboard focus
         if event.text.starts_with(key_codes::Tab)
@@ -670,14 +673,15 @@
             self.focus_next_item();
         } else if (event.text.starts_with(key_codes::Backtab)
             || (event.text.starts_with(key_codes::Tab) && event.modifiers.shift))
             && event.event_type == KeyEventType::KeyPressed
         {
             self.focus_previous_item();
         }
+        crate::properties::ChangeTracker::run_change_handlers();
     }
 
     /// Installs a binding on the specified property that's toggled whenever the text cursor is supposed to be visible or not.
     pub fn set_cursor_blink_binding(&self, prop: &crate::Property<bool>) {
         let existing_blinker = self.cursor_blinker.borrow().clone();
 
         let blinker = existing_blinker.upgrade().unwrap_or_else(|| {
@@ -687,21 +691,32 @@
             new_blinker
         });
 
         TextCursorBlinker::set_binding(blinker, prop);
     }
 
     /// Sets the focus to the item pointed to by item_ptr. This will remove the focus from any
-    /// currently focused item.
-    pub fn set_focus_item(&self, focus_item: &ItemRc) {
+    /// currently focused item. If set_focus is false, the focus is cleared.
+    pub fn set_focus_item(&self, new_focus_item: &ItemRc, set_focus: bool) {
         if self.prevent_focus_change.get() {
             return;
         }
+        if !set_focus {
+            let current_focus_item = self.focus_item.borrow().clone();
+            if let Some(current_focus_item_rc) = current_focus_item.upgrade() {
+                if current_focus_item_rc != *new_focus_item {
+                    // can't clear focus unless called with currently focused item.
+                    return;
+                }
+            }
+        }
+
         let old = self.take_focus_item();
-        let new = self.move_focus(focus_item.clone(), next_focus_item);
+        let new =
+            if set_focus { self.move_focus(new_focus_item.clone(), next_focus_item) } else { None };
         let window_adapter = self.window_adapter();
         if let Some(window_adapter) = window_adapter.internal(crate::InternalToken) {
             window_adapter.handle_focus_change(old, new);
         }
     }
 
     /// Take the focus_item out of this Window
@@ -994,15 +1009,15 @@
                         let popup_component = ItemTreeRc::borrow_pin(&current_popup.component);
                         popup_component.as_ref().item_geometry(0)
                     })
                     .translate(offset.to_vector());
 
                     if !popup_region.is_empty() {
                         let window_adapter = self.window_adapter();
-                        window_adapter.renderer().mark_dirty_region(popup_region.to_box2d());
+                        window_adapter.renderer().mark_dirty_region(popup_region.into());
                         window_adapter.request_redraw();
                     }
                 }
                 PopupWindowLocation::TopLevel(adapter) => {
                     let _ = adapter.set_visible(false);
                 }
             }
@@ -1246,17 +1261,18 @@
     }
 
     /// Sets the focus item.
     #[no_mangle]
     pub unsafe extern "C" fn slint_windowrc_set_focus_item(
         handle: *const WindowAdapterRcOpaque,
         focus_item: &ItemRc,
+        set_focus: bool,
     ) {
         let window_adapter = &*(handle as *const Rc<dyn WindowAdapter>);
-        WindowInner::from_pub(window_adapter.window()).set_focus_item(focus_item)
+        WindowInner::from_pub(window_adapter.window()).set_focus_item(focus_item, set_focus)
     }
 
     /// Associates the window with the given component.
     #[no_mangle]
     pub unsafe extern "C" fn slint_windowrc_set_component(
         handle: *const WindowAdapterRcOpaque,
         component: &ItemTreeRc,
```

### Comparing `slint-1.6.0a6/internal/compiler/Cargo.toml` & `slint-1.6.0a7/internal/compiler/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/LICENSES/Apache-2.0.txt` & `slint-1.6.0a7/internal/compiler/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/LICENSES/CC-BY-ND-4.0.txt` & `slint-1.6.0a7/internal/compiler/LICENSES/CC-BY-ND-4.0.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/LICENSES/GPL-3.0-only.txt` & `slint-1.6.0a7/internal/compiler/LICENSES/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md` & `slint-1.6.0a7/internal/compiler/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/LICENSES/LicenseRef-Slint-commercial.md` & `slint-1.6.0a7/internal/compiler/LICENSES/LicenseRef-Slint-commercial.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/LICENSES/MIT.txt` & `slint-1.6.0a7/internal/backends/linuxkms/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/README.md` & `slint-1.6.0a7/internal/compiler/README.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/build.rs` & `slint-1.6.0a7/internal/compiler/build.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/builtin_macros.rs` & `slint-1.6.0a7/internal/compiler/builtin_macros.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/builtins.slint` & `slint-1.6.0a7/internal/compiler/builtins.slint`

 * *Files 0% similar despite different names*

```diff
@@ -98,14 +98,17 @@
     in property <int> font-weight;
     in property <brush> color;  // StyleMetrics.default-text-color  set in apply_default_properties_from_style
     in property <TextHorizontalAlignment> horizontal-alignment;
     in property <TextVerticalAlignment> vertical-alignment;
     in property <TextOverflow> overflow;
     in property <TextWrap> wrap;
     in property <length> letter-spacing;
+    in property <brush> stroke;
+    in property <length> stroke-width;
+    in property <TextStrokeStyle> stroke-style;
     //-default_size_binding:implicit_size
 }
 
 export component TouchArea {
     in property <bool> enabled: true;
     out property <bool> pressed;
     out property <bool> has_hover;
```

### Comparing `slint-1.6.0a6/internal/compiler/diagnostics.rs` & `slint-1.6.0a7/internal/compiler/diagnostics.rs`

 * *Files 1% similar despite different names*

```diff
@@ -298,14 +298,17 @@
     }
 }
 
 #[derive(Default)]
 pub struct BuildDiagnostics {
     inner: Vec<Diagnostic>,
 
+    /// When false, throw error for experimental features
+    pub enable_experimental: bool,
+
     /// This is the list of all loaded files (with or without diagnostic)
     /// does not include the main file.
     /// FIXME: this doesn't really belong in the diagnostics, it should be somehow returned in another way
     /// (maybe in a compilation state that include the diagnostics?)
     pub all_loaded_files: Vec<PathBuf>,
 }
```

### Comparing `slint-1.6.0a6/internal/compiler/embedded_resources.rs` & `slint-1.6.0a7/internal/compiler/embedded_resources.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/expression_tree.rs` & `slint-1.6.0a7/internal/compiler/expression_tree.rs`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     Tan,
     ACos,
     ASin,
     ATan,
     Log,
     Pow,
     SetFocusItem,
+    ClearFocusItem,
     ShowPopupWindow,
     ClosePopupWindow,
     SetSelectionOffsets,
     /// A function that belongs to an item (such as TextInput's select-all function).
     ItemMemberFunction(String),
     /// the "42".to_float()
     StringToFloat,
@@ -129,14 +130,18 @@
                 return_type: Box::new(Type::Float32),
                 args: vec![Type::Float32, Type::Float32],
             },
             BuiltinFunction::SetFocusItem => Type::Function {
                 return_type: Box::new(Type::Void),
                 args: vec![Type::ElementReference],
             },
+            BuiltinFunction::ClearFocusItem => Type::Function {
+                return_type: Box::new(Type::Void),
+                args: vec![Type::ElementReference],
+            },
             BuiltinFunction::ShowPopupWindow | BuiltinFunction::ClosePopupWindow => {
                 Type::Function {
                     return_type: Box::new(Type::Void),
                     args: vec![Type::ElementReference],
                 }
             }
             BuiltinFunction::SetSelectionOffsets => Type::Function {
@@ -288,15 +293,15 @@
             | BuiltinFunction::Sin
             | BuiltinFunction::Tan
             | BuiltinFunction::ACos
             | BuiltinFunction::ASin
             | BuiltinFunction::Log
             | BuiltinFunction::Pow
             | BuiltinFunction::ATan => true,
-            BuiltinFunction::SetFocusItem => false,
+            BuiltinFunction::SetFocusItem | BuiltinFunction::ClearFocusItem => false,
             BuiltinFunction::ShowPopupWindow | BuiltinFunction::ClosePopupWindow => false,
             BuiltinFunction::SetSelectionOffsets => false,
             BuiltinFunction::ItemMemberFunction(..) => false,
             BuiltinFunction::StringToFloat | BuiltinFunction::StringIsFloat => true,
             BuiltinFunction::ColorRgbaStruct
             | BuiltinFunction::ColorHsvaStruct
             | BuiltinFunction::ColorBrighter
@@ -345,15 +350,15 @@
             | BuiltinFunction::Sin
             | BuiltinFunction::Tan
             | BuiltinFunction::ACos
             | BuiltinFunction::ASin
             | BuiltinFunction::Log
             | BuiltinFunction::Pow
             | BuiltinFunction::ATan => true,
-            BuiltinFunction::SetFocusItem => false,
+            BuiltinFunction::SetFocusItem | BuiltinFunction::ClearFocusItem => false,
             BuiltinFunction::ShowPopupWindow | BuiltinFunction::ClosePopupWindow => false,
             BuiltinFunction::SetSelectionOffsets => false,
             BuiltinFunction::ItemMemberFunction(..) => false,
             BuiltinFunction::StringToFloat | BuiltinFunction::StringIsFloat => true,
             BuiltinFunction::ColorRgbaStruct
             | BuiltinFunction::ColorHsvaStruct
             | BuiltinFunction::ColorBrighter
```

### Comparing `slint-1.6.0a6/internal/compiler/fileaccess.rs` & `slint-1.6.0a7/internal/compiler/fileaccess.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/generator/cpp.rs` & `slint-1.6.0a7/internal/compiler/generator/cpp.rs`

 * *Files 0% similar despite different names*

```diff
@@ -85,14 +85,16 @@
         pub namespace: Option<String>,
         pub declarations: Vec<Declaration>,
         pub definitions: Vec<Declaration>,
     }
 
     impl Display for File {
         fn fmt(&self, f: &mut Formatter<'_>) -> Result<(), Error> {
+            writeln!(f, "// This file is auto-generated")?;
+            writeln!(f, "#pragma once")?;
             for i in &self.includes {
                 writeln!(f, "#include {}", i)?;
             }
             if let Some(namespace) = &self.namespace {
                 writeln!(f, "namespace {} {{", namespace)?;
                 INDENTATION.with(|x| x.set(x.get() + 1));
             }
@@ -1351,19 +1353,19 @@
     ));
 
     target_struct.members.push((
         Access::Private,
         Declaration::Function(Function {
             name: "accessible_string_property".into(),
             signature:
-                "([[maybe_unused]] slint::private_api::ItemTreeRef component, uint32_t index, slint::cbindgen_private::AccessibleStringProperty what, slint::SharedString *result) -> void"
+                "([[maybe_unused]] slint::private_api::ItemTreeRef component, uint32_t index, slint::cbindgen_private::AccessibleStringProperty what, slint::SharedString *result) -> bool"
                     .into(),
             is_static: true,
             statements: Some(vec![format!(
-                "*result = reinterpret_cast<const {}*>(component.instance)->accessible_string_property(index, what);",
+                "if (auto r = reinterpret_cast<const {}*>(component.instance)->accessible_string_property(index, what)) {{ *result = *r; return true; }} else {{ return false; }}",
                 item_tree_class_name
             )]),
             ..Default::default()
         }),
     ));
 
     target_struct.members.push((
@@ -1619,14 +1621,25 @@
 
         target_struct.members.push((
             field_access,
             Declaration::Var(Var { ty, name: cpp_name, ..Default::default() }),
         ));
     }
 
+    for (i, _) in component.change_callbacks.iter().enumerate() {
+        target_struct.members.push((
+            field_access,
+            Declaration::Var(Var {
+                ty: "slint::private_api::ChangeTracker".into(),
+                name: format!("change_tracker{}", i),
+                ..Default::default()
+            }),
+        ));
+    }
+
     let mut user_init = vec!["[[maybe_unused]] auto self = this;".into()];
 
     let mut children_visitor_cases = Vec::new();
     let mut subtrees_ranges_cases = Vec::new();
     let mut subtrees_components_cases = Vec::new();
 
     for sub in &component.sub_components {
@@ -1822,14 +1835,20 @@
 
     user_init.extend(component.init_code.iter().map(|e| {
         let mut expr_str = compile_expression(&e.borrow(), &ctx);
         expr_str.push(';');
         expr_str
     }));
 
+    user_init.extend(component.change_callbacks.iter().enumerate().map(|(idx, (p, e))| {
+        let code = compile_expression(&e.borrow(), &ctx);
+        let prop = compile_expression(&llr::Expression::PropertyReference(p.clone()), &ctx);
+        format!("self->change_tracker{idx}.init(self, [](auto self) {{ return {prop}; }}, [](auto self, auto) {{ {code}; }});")
+    }));
+
     target_struct
         .members
         .extend(generate_functions(&component.functions, &ctx).map(|x| (Access::Public, x)));
 
     target_struct.members.push((
         field_access,
         Declaration::Function(Function {
@@ -1973,15 +1992,15 @@
         "accessible_role",
         "(uint32_t index) const -> slint::cbindgen_private::AccessibleRole",
         "",
         accessible_role_cases,
     );
     dispatch_item_function(
         "accessible_string_property",
-        "(uint32_t index, slint::cbindgen_private::AccessibleStringProperty what) const -> slint::SharedString",
+        "(uint32_t index, slint::cbindgen_private::AccessibleStringProperty what) const -> std::optional<slint::SharedString>",
         ", what",
         accessible_string_cases,
     );
 
     dispatch_item_function(
         "accessibility_action",
         "(uint32_t index, const slint::cbindgen_private::AccessibilityAction &action) const",
@@ -3094,19 +3113,28 @@
             ctx.generator_state.conditional_includes.cmath.set(true);
             format!("std::atan({}) / {}", a.next().unwrap(), pi_180)
         }
         BuiltinFunction::SetFocusItem => {
             if let [llr::Expression::PropertyReference(pr)] = arguments {
                 let window = access_window_field(ctx);
                 let focus_item = access_item_rc(pr, ctx);
-                format!("{}.set_focus_item({});", window, focus_item)
+                format!("{}.set_focus_item({}, true);", window, focus_item)
             } else {
                 panic!("internal error: invalid args to SetFocusItem {:?}", arguments)
             }
         }
+        BuiltinFunction::ClearFocusItem => {
+            if let [llr::Expression::PropertyReference(pr)] = arguments {
+                let window = access_window_field(ctx);
+                let focus_item = access_item_rc(pr, ctx);
+                format!("{}.set_focus_item({}, false);", window, focus_item)
+            } else {
+                panic!("internal error: invalid args to ClearFocusItem {:?}", arguments)
+            }
+        }
         /*  std::from_chars is unfortunately not yet implemented in gcc
         BuiltinFunction::StringIsFloat => {
             "[](const auto &a){ double v; auto r = std::from_chars(std::begin(a), std::end(a), v); return r.ptr == std::end(a); }"
                 .into()
         }
         BuiltinFunction::StringToFloat => {
             "[](const auto &a){ double v; auto r = std::from_chars(std::begin(a), std::end(a), v); return r.ptr == std::end(a) ? v : 0; }"
```

### Comparing `slint-1.6.0a6/internal/compiler/generator/rust.rs` & `slint-1.6.0a7/internal/compiler/generator/rust.rs`

 * *Files 1% similar despite different names*

```diff
@@ -628,14 +628,20 @@
         } else {
             let rust_property_type = rust_property_type(&property.ty).unwrap();
             declared_property_vars.push(prop_ident.clone());
             declared_property_types.push(rust_property_type.clone());
         }
     }
 
+    let change_tracker_names = component
+        .change_callbacks
+        .iter()
+        .enumerate()
+        .map(|(idx, _)| format_ident!("change_tracker{idx}"));
+
     let declared_functions = generate_functions(&component.functions, &ctx);
 
     let mut init = vec![];
     let mut item_names = vec![];
     let mut item_types = vec![];
 
     #[cfg(slint_debug_property)]
@@ -802,15 +808,15 @@
             } else {
                 quote!((#index, sp::AccessibilityAction::#what) => { #e })
             });
             supported_accessibility_actions.entry(*index).or_default().insert(what);
         } else {
             let what = ident(what);
             accessible_string_property_branch
-                .push(quote!((#index, sp::AccessibleStringProperty::#what) => #e,));
+                .push(quote!((#index, sp::AccessibleStringProperty::#what) => sp::Some(#e),));
         }
     }
     let mut supported_accessibility_actions_branch = supported_accessibility_actions
         .into_iter()
         .map(|(index, values)| quote!(#index => #(sp::SupportedAccessibilityAction::#values)|*,))
         .collect::<Vec<_>>();
 
@@ -956,14 +962,36 @@
     });
 
     user_init_code.extend(component.init_code.iter().map(|e| {
         let code = compile_expression(&e.borrow(), &ctx);
         quote!(#code;)
     }));
 
+    user_init_code.extend(component.change_callbacks.iter().enumerate().map(|(idx, (p, e))| {
+        let code = compile_expression(&e.borrow(), &ctx);
+        let prop = compile_expression(&Expression::PropertyReference(p.clone()), &ctx);
+        let change_tracker = format_ident!("change_tracker{idx}");
+        quote! {
+            let self_weak = sp::VRcMapped::downgrade(&self_rc);
+            _self.#change_tracker.init(
+                self_weak,
+                move |self_weak| {
+                    let self_rc = self_weak.upgrade().unwrap();
+                    let _self = self_rc.as_pin_ref();
+                    #prop
+                },
+                move |self_weak, _| {
+                    let self_rc = self_weak.upgrade().unwrap();
+                    let _self = self_rc.as_pin_ref();
+                    #code;
+                }
+            );
+        }
+    }));
+
     let layout_info_h = compile_expression(&component.layout_info_h.borrow(), &ctx);
     let layout_info_v = compile_expression(&component.layout_info_v.borrow(), &ctx);
 
     // FIXME! this is only public because of the ComponentHandle::Inner. we should find another way
     let visibility =
         core::ptr::eq(&root.item_tree.root as *const _, component as *const _).then(|| quote!(pub));
 
@@ -987,14 +1015,15 @@
         #visibility
         struct #inner_component_id {
             #(#item_names : sp::#item_types,)*
             #(#sub_component_names : #sub_component_types,)*
             #(#declared_property_vars : sp::Property<#declared_property_types>,)*
             #(#declared_callbacks : sp::Callback<(#(#declared_callbacks_types,)*), #declared_callbacks_ret>,)*
             #(#repeated_element_names : sp::Repeater<#repeated_element_components>,)*
+            #(#change_tracker_names : sp::ChangeTracker,)*
             self_weak : sp::OnceCell<sp::VWeakMapped<sp::ItemTreeVTable, #inner_component_id>>,
             #(parent : #parent_component_type,)*
             root : sp::OnceCell<sp::VWeak<sp::ItemTreeVTable, #root_component_id>>,
             tree_index: ::core::cell::Cell<u32>,
             tree_index_of_first_child: ::core::cell::Cell<u32>,
             #extra_fields
         }
@@ -1086,20 +1115,20 @@
                 }
             }
 
             fn accessible_string_property(
                 self: ::core::pin::Pin<&Self>,
                 index: u32,
                 what: sp::AccessibleStringProperty,
-            ) -> sp::SharedString {
+            ) -> sp::Option<sp::SharedString> {
                 #![allow(unused)]
                 let _self = self;
                 match (index, what) {
                     #(#accessible_string_property_branch)*
-                    _ => ::core::default::Default::default(),
+                    _ => sp::None,
                 }
             }
 
             fn accessibility_action(self: ::core::pin::Pin<&Self>, index: u32, action: &sp::AccessibilityAction) {
                 #![allow(unused)]
                 let _self = self;
                 match (index, action) {
@@ -1554,16 +1583,21 @@
             }
 
             fn accessible_string_property(
                 self: ::core::pin::Pin<&Self>,
                 index: u32,
                 what: sp::AccessibleStringProperty,
                 result: &mut sp::SharedString,
-            ) {
-                *result = self.accessible_string_property(index, what);
+            ) -> bool {
+                if let Some(r) = self.accessible_string_property(index, what) {
+                    *result = r;
+                    true
+                } else {
+                    false
+                }
             }
 
             fn accessibility_action(self: ::core::pin::Pin<&Self>, index: u32, action: &sp::AccessibilityAction) {
                 self.accessibility_action(index, action);
             }
 
             fn supported_accessibility_actions(self: ::core::pin::Pin<&Self>, index: u32) -> sp::SupportedAccessibilityAction {
@@ -2387,20 +2421,31 @@
     let mut a = arguments.iter().map(|a| compile_expression(a, ctx));
     match function {
         BuiltinFunction::SetFocusItem => {
             if let [Expression::PropertyReference(pr)] = arguments {
                 let window_tokens = access_window_adapter_field(ctx);
                 let focus_item = access_item_rc(pr, ctx);
                 quote!(
-                    sp::WindowInner::from_pub(#window_tokens.window()).set_focus_item(#focus_item)
+                    sp::WindowInner::from_pub(#window_tokens.window()).set_focus_item(#focus_item, true)
                 )
             } else {
                 panic!("internal error: invalid args to SetFocusItem {:?}", arguments)
             }
         }
+        BuiltinFunction::ClearFocusItem => {
+            if let [Expression::PropertyReference(pr)] = arguments {
+                let window_tokens = access_window_adapter_field(ctx);
+                let focus_item = access_item_rc(pr, ctx);
+                quote!(
+                    sp::WindowInner::from_pub(#window_tokens.window()).set_focus_item(#focus_item, false)
+                )
+            } else {
+                panic!("internal error: invalid args to ClearFocusItem {:?}", arguments)
+            }
+        }
         BuiltinFunction::ShowPopupWindow => {
             if let [Expression::NumberLiteral(popup_index), x, y, close_on_click, Expression::PropertyReference(parent_ref)] =
                 arguments
             {
                 let mut parent_ctx = ctx;
                 let mut component_access_tokens = quote!(_self);
                 if let llr::PropertyReference::InParent { level, .. } = parent_ref {
```

### Comparing `slint-1.6.0a6/internal/compiler/generator.rs` & `slint-1.6.0a7/internal/compiler/generator.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/langtype.rs` & `slint-1.6.0a7/internal/compiler/langtype.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/layout.rs` & `slint-1.6.0a7/internal/compiler/layout.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/lexer.rs` & `slint-1.6.0a7/internal/compiler/lexer.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/lib.rs` & `slint-1.6.0a7/internal/compiler/lib.rs`

 * *Files 4% similar despite different names*

```diff
@@ -85,16 +85,16 @@
 
     /// Compile time scale factor to apply to embedded resources such as images and glyphs.
     pub scale_factor: f64,
 
     /// expose the accessible role and properties
     pub accessibility: bool,
 
-    /// Add support for component containers
-    pub enable_component_containers: bool,
+    /// Add support for experimental features
+    pub enable_experimental: bool,
 
     /// The domain used as one of the parameter to the translate function
     pub translation_domain: Option<String>,
 
     /// C++ namespace
     pub cpp_namespace: Option<String>,
 }
@@ -136,18 +136,15 @@
 
         let scale_factor = std::env::var("SLINT_SCALE_FACTOR")
             .ok()
             .and_then(|x| x.parse::<f64>().ok())
             .filter(|f| *f > 0.)
             .unwrap_or(1.);
 
-        let enable_experimental_features =
-            std::env::var_os("SLINT_ENABLE_EXPERIMENTAL_FEATURES").is_some();
-
-        let enable_component_containers = enable_experimental_features;
+        let enable_experimental = std::env::var_os("SLINT_ENABLE_EXPERIMENTAL_FEATURES").is_some();
 
         let cpp_namespace = match output_format {
             #[cfg(feature = "cpp")]
             crate::generator::OutputFormat::Cpp(config) => match config.namespace {
                 Some(namespace) => Some(namespace),
                 None => match std::env::var("SLINT_CPP_NAMESPACE") {
                     Ok(namespace) => Some(namespace),
@@ -163,15 +160,15 @@
             library_paths: Default::default(),
             style: Default::default(),
             open_import_fallback: None,
             resource_url_mapper: None,
             inline_all_elements,
             scale_factor,
             accessibility: true,
-            enable_component_containers,
+            enable_experimental,
             translation_domain: None,
             cpp_namespace,
         }
     }
 }
 
 fn prepare_for_compile(
@@ -181,15 +178,17 @@
     #[cfg(feature = "software-renderer")]
     if compiler_config.embed_resources == EmbedResourcesKind::EmbedTextures {
         // HACK: disable accessibility when compiling for the software renderer
         // accessibility is not supported with backend that support software renderer anyway
         compiler_config.accessibility = false;
     }
 
-    let global_type_registry = if compiler_config.enable_component_containers {
+    diagnostics.enable_experimental = compiler_config.enable_experimental;
+
+    let global_type_registry = if compiler_config.enable_experimental {
         crate::typeregister::TypeRegister::builtin_experimental()
     } else {
         crate::typeregister::TypeRegister::builtin()
     };
 
     typeloader::TypeLoader::new(global_type_registry, compiler_config, diagnostics)
 }
```

### Comparing `slint-1.6.0a6/internal/compiler/literals.rs` & `slint-1.6.0a7/internal/compiler/literals.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/llr/expression.rs` & `slint-1.6.0a7/internal/compiler/llr/expression.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/llr/item_tree.rs` & `slint-1.6.0a7/internal/compiler/llr/item_tree.rs`

 * *Files 1% similar despite different names*

```diff
@@ -232,14 +232,15 @@
     pub repeated: Vec<RepeatedElement>,
     pub component_containers: Vec<ComponentContainerElement>,
     pub popup_windows: Vec<ItemTree>,
     pub sub_components: Vec<SubComponentInstance>,
     /// The initial value or binding for properties.
     /// This is ordered in the order they must be set.
     pub property_init: Vec<(PropertyReference, BindingExpression)>,
+    pub change_callbacks: Vec<(PropertyReference, MutExpression)>,
     /// The animation for properties which are animated
     pub animations: HashMap<PropertyReference, Expression>,
     pub two_way_bindings: Vec<(PropertyReference, PropertyReference)>,
     pub const_properties: Vec<PropertyReference>,
     /// Code that is run in the sub component constructor, after property initializations
     pub init_code: Vec<MutExpression>,
 
@@ -368,14 +369,17 @@
             visitor(&sc.layout_info_v, ctx);
             for e in sc.accessible_prop.values() {
                 visitor(e, ctx);
             }
             for i in sc.geometries.iter().flatten() {
                 visitor(i, ctx);
             }
+            for (_, e) in sc.change_callbacks.iter() {
+                visitor(e, ctx);
+            }
         });
         for g in &self.globals {
             let ctx = EvaluationContext::new_global(self, g, ());
             for e in g.init_values.iter().filter_map(|x| x.as_ref()) {
                 visitor(&e.expression, &ctx)
             }
         }
```

### Comparing `slint-1.6.0a6/internal/compiler/llr/lower_expression.rs` & `slint-1.6.0a7/internal/compiler/llr/lower_expression.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/llr/lower_to_item_tree.rs` & `slint-1.6.0a7/internal/compiler/llr/lower_to_item_tree.rs`

 * *Files 1% similar despite different names*

```diff
@@ -187,14 +187,15 @@
         functions: Default::default(),
         items: Default::default(),
         repeated: Default::default(),
         component_containers: Default::default(),
         popup_windows: Default::default(),
         sub_components: Default::default(),
         property_init: Default::default(),
+        change_callbacks: Default::default(),
         animations: Default::default(),
         two_way_bindings: Default::default(),
         const_properties: Default::default(),
         init_code: Default::default(),
         geometries: Default::default(),
         // just initialize to dummy expression right now and it will be set later
         layout_info_h: super::Expression::BoolLiteral(false).into(),
@@ -202,14 +203,15 @@
         accessible_prop: Default::default(),
         prop_analysis: Default::default(),
     };
     let mut mapping = LoweredSubComponentMapping::default();
     let mut repeated = vec![];
     let mut component_container_data = vec![];
     let mut accessible_prop = Vec::new();
+    let mut change_callbacks = Vec::new();
 
     if let Some(parent) = component.parent_element.upgrade() {
         // Add properties for the model data and index
         if parent.borrow().repeated.as_ref().map_or(false, |x| !x.is_conditional_element) {
             sub_component.properties.push(Property {
                 name: "model_data".into(),
                 ty: crate::expression_tree::Expression::RepeaterModelReference {
@@ -314,14 +316,19 @@
         };
         for (key, nr) in &elem.accessibility_props.0 {
             // TODO: we also want to split by type (role/string/...)
             let enum_value =
                 crate::generator::to_pascal_case(key.strip_prefix("accessible-").unwrap());
             accessible_prop.push((*elem.item_index.get().unwrap(), enum_value, nr.clone()));
         }
+
+        for (prop, expr) in &elem.change_callbacks {
+            change_callbacks.push((NamedReference::new(&element, prop), expr.borrow().clone()));
+        }
+
         Some(element.clone())
     });
     let ctx = ExpressionContext { mapping: &mapping, state, parent: parent_context, component };
     crate::generator::handle_property_bindings_init(component, |e, p, binding| {
         let nr = NamedReference::new(e, p);
         let prop = ctx.map_property_reference(&nr);
 
@@ -467,14 +474,24 @@
                 _ => panic!("Invalid type for accessible property"),
             };
 
             ((idx, key), expr.into())
         })
         .collect();
 
+    sub_component.change_callbacks = change_callbacks
+        .into_iter()
+        .map(|(nr, exprs)| {
+            let prop = ctx.map_property_reference(&nr);
+            let expr =
+                super::lower_expression::lower_expression(&tree_Expression::CodeBlock(exprs), &ctx);
+            (prop, expr.into())
+        })
+        .collect();
+
     crate::object_tree::recurse_elem(&component.root_element, &(), &mut |element, _| {
         let elem = element.borrow();
         if elem.repeated.is_some() {
             return;
         };
         let Some(geom) = &elem.geometry_props else { return };
         let item_index = *elem.item_index.get().unwrap() as usize;
```

### Comparing `slint-1.6.0a6/internal/compiler/llr/optim_passes/count_property_use.rs` & `slint-1.6.0a7/internal/compiler/llr/optim_passes/count_property_use.rs`

 * *Files 3% similar despite different names*

```diff
@@ -106,14 +106,20 @@
             visit_property(b, ctx);
         }
 
         // 8.functions (TODO: only visit used function)
         for f in &sc.functions {
             f.code.visit_recursive(&mut |e| visit_expression(e, ctx));
         }
+
+        // 9. change callbacks
+        for (p, e) in &sc.change_callbacks {
+            visit_property(p, ctx);
+            e.visit_recursive(&mut |e| visit_expression(e, ctx));
+        }
     });
 
     // TODO: only visit used function
     for g in root.globals.iter() {
         let ctx = EvaluationContext::new_global(root, g, ());
         for f in &g.functions {
             f.code.visit_recursive(&mut |e| visit_expression(e, &ctx));
```

### Comparing `slint-1.6.0a6/internal/compiler/llr/optim_passes/inline_expressions.rs` & `slint-1.6.0a7/internal/compiler/llr/optim_passes/inline_expressions.rs`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         BuiltinFunction::Sin => 10,
         BuiltinFunction::Tan => 10,
         BuiltinFunction::ACos => 10,
         BuiltinFunction::ASin => 10,
         BuiltinFunction::ATan => 10,
         BuiltinFunction::Log => 10,
         BuiltinFunction::Pow => 10,
-        BuiltinFunction::SetFocusItem => isize::MAX,
+        BuiltinFunction::SetFocusItem | BuiltinFunction::ClearFocusItem => isize::MAX,
         BuiltinFunction::ShowPopupWindow | BuiltinFunction::ClosePopupWindow => isize::MAX,
         BuiltinFunction::SetSelectionOffsets => isize::MAX,
         BuiltinFunction::ItemMemberFunction(..) => isize::MAX,
         BuiltinFunction::StringToFloat => 50,
         BuiltinFunction::StringIsFloat => 50,
         BuiltinFunction::ColorRgbaStruct => 50,
         BuiltinFunction::ColorHsvaStruct => 50,
```

### Comparing `slint-1.6.0a6/internal/compiler/llr/pretty_print.rs` & `slint-1.6.0a7/internal/compiler/llr/pretty_print.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/llr.rs` & `slint-1.6.0a7/internal/compiler/llr.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/load_builtins.rs` & `slint-1.6.0a7/internal/compiler/load_builtins.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/lookup.rs` & `slint-1.6.0a7/internal/compiler/lookup.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/namedreference.rs` & `slint-1.6.0a7/internal/compiler/namedreference.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/object_tree.rs` & `slint-1.6.0a7/internal/compiler/object_tree.rs`

 * *Files 1% similar despite different names*

```diff
@@ -595,14 +595,15 @@
     /// After inlining there can be duplicated id in the component.
     /// The id are then re-assigned unique id in the assign_id pass
     pub id: String,
     //pub base: QualifiedTypeName,
     pub base_type: ElementType,
     /// Currently contains also the callbacks. FIXME: should that be changed?
     pub bindings: BindingsMap,
+    pub change_callbacks: BTreeMap<String, RefCell<Vec<Expression>>>,
     pub property_analysis: RefCell<HashMap<String, PropertyAnalysis>>,
 
     pub children: Vec<ElementRc>,
     /// The component which contains this element.
     pub enclosing_component: Weak<Component>,
 
     pub property_declarations: BTreeMap<String, PropertyDeclaration>,
@@ -682,14 +683,15 @@
     indentation: usize,
 ) -> std::fmt::Result {
     if let Some(repeated) = &e.repeated {
         write!(f, "for {}[{}] in ", repeated.model_data_id, repeated.index_id)?;
         expression_tree::pretty_print(f, &repeated.model)?;
         write!(f, ":")?;
         if let ElementType::Component(base) = &e.base_type {
+            write!(f, "(base) ")?;
             if base.parent_element.upgrade().is_some() {
                 pretty_print(f, &base.root_element.borrow(), indentation)?;
                 return Ok(());
             }
         }
     }
     if e.is_component_placeholder {
@@ -727,14 +729,22 @@
             writeln!(f, "animate {} {:?}", name, anim)?;
         }
         for nr in &expr.two_way_bindings {
             indent!();
             writeln!(f, "{} <=> {:?};", name, nr)?;
         }
     }
+    for (name, ch) in &e.change_callbacks {
+        for ex in &*ch.borrow() {
+            indent!();
+            writeln!(f, "changed {name} => {{ ")?;
+            expression_tree::pretty_print(f, ex)?;
+            writeln!(f, "  }}")?;
+        }
+    }
     if !e.states.is_empty() {
         indent!();
         writeln!(f, "states {:?}", e.states)?;
     }
     if !e.transitions.is_empty() {
         indent!();
         writeln!(f, "transitions {:?} ", e.transitions)?;
@@ -1279,14 +1289,46 @@
                         "Can only refer to property in the current element".into(),
                         &prop_name_token,
                     ),
                 }
             }
         }
 
+        for ch in node.PropertyChangedCallback() {
+            if !diag.enable_experimental {
+                diag.push_error(
+                    "Change callbacks are experimental and not yet implemented in this version of Slint".into(),
+                    &ch,
+                );
+            }
+            let Some(prop) = parser::identifier_text(&ch.DeclaredIdentifier()) else { continue };
+            let lookup_result = r.lookup_property(&prop);
+            if lookup_result.property_visibility == PropertyVisibility::Private
+                && !lookup_result.is_local_to_component
+            {
+                diag.push_error(
+                    format!("Change callback on a private property '{prop}'"),
+                    &ch.DeclaredIdentifier(),
+                );
+            }
+            let handler = Expression::Uncompiled(ch.clone().into());
+            match r.change_callbacks.entry(prop) {
+                Entry::Vacant(e) => {
+                    e.insert(vec![handler].into());
+                }
+                Entry::Occupied(mut e) => {
+                    diag.push_error(
+                        format!("Duplicated change callback on '{}'", e.key()),
+                        &ch.DeclaredIdentifier(),
+                    );
+                    e.get_mut().get_mut().push(handler);
+                }
+            }
+        }
+
         let mut children_placeholder = None;
         let r = r.make_rc();
 
         for se in node.children() {
             if se.kind() == SyntaxKind::SubElement {
                 let parent_type = r.borrow().base_type.clone();
                 r.borrow_mut().children.push(Element::from_sub_element_node(
@@ -2042,14 +2084,21 @@
         .as_mut()
         .map(|r| (std::mem::take(&mut r.model), r.is_conditional_element));
     if let Some((mut model, is_cond)) = repeated {
         vis(&mut model, None, &|| if is_cond { Type::Bool } else { Type::Model });
         elem.borrow_mut().repeated.as_mut().unwrap().model = model;
     }
     visit_element_expressions_simple(elem, &mut vis);
+
+    for (_, expr) in &elem.borrow().change_callbacks {
+        for expr in expr.borrow_mut().iter_mut() {
+            vis(expr, Some("$change callback$"), &|| Type::Void);
+        }
+    }
+
     let mut states = std::mem::take(&mut elem.borrow_mut().states);
     for s in &mut states {
         if let Some(cond) = s.condition.as_mut() {
             vis(cond, None, &|| Type::Bool)
         }
         for (ne, e, _) in &mut s.property_changes {
             vis(e, Some(ne.name()), &|| {
```

### Comparing `slint-1.6.0a6/internal/compiler/parser/document.rs` & `slint-1.6.0a7/internal/compiler/parser/document.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/parser/element.rs` & `slint-1.6.0a7/internal/compiler/parser/element.rs`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 /// callback foobar;
 /// property<int> width;
 /// animate someProp { }
 /// animate * { }
 /// @children
 /// double_binding <=> element.property;
 /// public pure function foo() {}
+/// changed foo => {}
 /// ```
 pub fn parse_element_content(p: &mut impl Parser) {
     let mut had_parse_error = false;
     loop {
         match p.nth(0).kind() {
             SyntaxKind::RBrace => return,
             SyntaxKind::Eof => return,
@@ -70,14 +71,17 @@
                             && p.nth(2).as_str() == "function") =>
                 {
                     parse_function(&mut *p);
                 }
                 SyntaxKind::Identifier | SyntaxKind::Star if p.peek().as_str() == "animate" => {
                     parse_property_animation(&mut *p);
                 }
+                SyntaxKind::Identifier if p.peek().as_str() == "changed" => {
+                    parse_changed_callback(&mut *p);
+                }
                 SyntaxKind::LAngle | SyntaxKind::Identifier if p.peek().as_str() == "property" => {
                     parse_property_declaration(&mut *p);
                 }
                 SyntaxKind::Identifier
                     if p.nth(1).as_str() == "property"
                         && matches!(
                             p.peek().as_str(),
@@ -434,14 +438,30 @@
                 p.error("Only bindings are allowed in animations");
             }
         }
     }
 }
 
 #[cfg_attr(test, parser_test)]
+/// ```test,PropertyChangedCallback
+/// changed the-property => { x = y; }
+/// ```
+fn parse_changed_callback(p: &mut impl Parser) {
+    debug_assert_eq!(p.peek().as_str(), "changed");
+    let mut p = p.start_node(SyntaxKind::PropertyChangedCallback);
+    p.expect(SyntaxKind::Identifier); // changed
+    {
+        let mut p = p.start_node(SyntaxKind::DeclaredIdentifier);
+        p.expect(SyntaxKind::Identifier);
+    }
+    p.expect(SyntaxKind::FatArrow);
+    parse_code_block(&mut *p);
+}
+
+#[cfg_attr(test, parser_test)]
 /// ```test,States
 /// states []
 /// states [ foo when bar : { x:y; } another_state : { x:z; }]
 /// ```
 fn parse_states(p: &mut impl Parser) {
     debug_assert_eq!(p.peek().as_str(), "states");
     let mut p = p.start_node(SyntaxKind::States);
```

### Comparing `slint-1.6.0a6/internal/compiler/parser/expressions.rs` & `slint-1.6.0a7/internal/compiler/parser/expressions.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/parser/statements.rs` & `slint-1.6.0a7/internal/compiler/parser/statements.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/parser/type.rs` & `slint-1.6.0a7/internal/compiler/parser/type.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/parser.rs` & `slint-1.6.0a7/internal/compiler/parser.rs`

 * *Files 1% similar despite different names*

```diff
@@ -328,29 +328,32 @@
     {
         Document -> [ *Component, *ExportsList, *ImportSpecifier, *StructDeclaration, *EnumDeclaration ],
         /// `DeclaredIdentifier := Element { ... }`
         Component -> [ DeclaredIdentifier, Element ],
         /// `id := Element { ... }`
         SubElement -> [ Element ],
         Element -> [ ?QualifiedName, *PropertyDeclaration, *Binding, *CallbackConnection,
-                     *CallbackDeclaration, *Function, *SubElement, *RepeatedElement, *PropertyAnimation,
+                     *CallbackDeclaration, *Function, *SubElement, *RepeatedElement,
+                     *PropertyAnimation, *PropertyChangedCallback,
                      *TwoWayBinding, *States, *Transitions, ?ChildrenPlaceholder ],
         RepeatedElement -> [ ?DeclaredIdentifier, ?RepeatedIndex, Expression , SubElement],
         RepeatedIndex -> [],
         ConditionalElement -> [ Expression , SubElement],
         CallbackDeclaration -> [ DeclaredIdentifier, *Type, ?ReturnType, ?TwoWayBinding ],
         Function -> [DeclaredIdentifier, *ArgumentDeclaration, ?ReturnType, CodeBlock ],
         ArgumentDeclaration -> [DeclaredIdentifier, Type],
         /// `-> type`  (but without the ->)
         ReturnType -> [Type],
         CallbackConnection -> [ *DeclaredIdentifier,  CodeBlock ],
         /// Declaration of a property.
         PropertyDeclaration-> [ ?Type , DeclaredIdentifier, ?BindingExpression, ?TwoWayBinding ],
         /// QualifiedName are the properties name
         PropertyAnimation-> [ *QualifiedName, *Binding ],
+        /// `changed xxx => {...}`  where `xxx` is the DeclaredIdentifier
+        PropertyChangedCallback-> [ DeclaredIdentifier, CodeBlock ],
         /// wraps Identifiers, like `Rectangle` or `SomeModule.SomeType`
         QualifiedName-> [],
         /// Wraps single identifier (to disambiguate when there are other identifier in the production)
         DeclaredIdentifier -> [],
         ChildrenPlaceholder -> [],
         Binding-> [ BindingExpression ],
         /// `xxx <=> something`
```

### Comparing `slint-1.6.0a6/internal/compiler/passes/apply_default_properties_from_style.rs` & `slint-1.6.0a7/internal/compiler/passes/apply_default_properties_from_style.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/passes/binding_analysis.rs` & `slint-1.6.0a7/internal/compiler/passes/binding_analysis.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/passes/border_radius.rs` & `slint-1.6.0a7/internal/compiler/passes/border_radius.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/passes/check_expressions.rs` & `slint-1.6.0a7/internal/compiler/passes/check_expressions.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/passes/check_public_api.rs` & `slint-1.6.0a7/internal/compiler/passes/check_public_api.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/passes/check_rotation.rs` & `slint-1.6.0a7/internal/compiler/passes/check_rotation.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/passes/clip.rs` & `slint-1.6.0a7/internal/compiler/passes/clip.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/passes/collect_custom_fonts.rs` & `slint-1.6.0a7/internal/compiler/passes/collect_custom_fonts.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/passes/collect_globals.rs` & `slint-1.6.0a7/internal/compiler/passes/collect_globals.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/passes/collect_init_code.rs` & `slint-1.6.0a7/internal/compiler/passes/collect_init_code.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/passes/collect_structs_and_enums.rs` & `slint-1.6.0a7/internal/compiler/passes/collect_structs_and_enums.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/passes/collect_subcomponents.rs` & `slint-1.6.0a7/internal/compiler/passes/collect_subcomponents.rs`

 * *Files 12% similar despite different names*

```diff
@@ -33,10 +33,17 @@
                     return;
                 }
                 base_comp.clone()
             }
             _ => return,
         };
         collect_subcomponents_recursive(&base_comp, result, hash);
+        if base_comp.parent_element.upgrade().is_some() {
+            // This is not a sub-component, but is a repeated component
+            return;
+        }
         result.push(base_comp);
     });
+    for popup in component.popup_windows.borrow().iter() {
+        collect_subcomponents_recursive(&popup.component, result, hash);
+    }
 }
```

### Comparing `slint-1.6.0a6/internal/compiler/passes/compile_paths.rs` & `slint-1.6.0a7/internal/compiler/passes/compile_paths.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/passes/const_propagation.rs` & `slint-1.6.0a7/internal/compiler/passes/const_propagation.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/passes/deduplicate_property_read.rs` & `slint-1.6.0a7/internal/compiler/passes/deduplicate_property_read.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/passes/default_geometry.rs` & `slint-1.6.0a7/internal/compiler/passes/default_geometry.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/passes/embed_glyphs.rs` & `slint-1.6.0a7/internal/compiler/passes/embed_glyphs.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/passes/embed_images.rs` & `slint-1.6.0a7/internal/compiler/passes/embed_images.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/passes/ensure_window.rs` & `slint-1.6.0a7/internal/compiler/passes/ensure_window.rs`

 * *Files 8% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
     // the old_root becomes the Window
     let mut win_elem_mut = win_elem.borrow_mut();
     let new_root = Element {
         id: std::mem::replace(&mut win_elem_mut.id, "root_window".into()),
         base_type: std::mem::replace(&mut win_elem_mut.base_type, window_type),
         bindings: Default::default(),
+        change_callbacks: Default::default(),
         is_component_placeholder: false,
         property_analysis: Default::default(),
         children: std::mem::take(&mut win_elem_mut.children),
         enclosing_component: win_elem_mut.enclosing_component.clone(),
         property_declarations: Default::default(),
         named_references: Default::default(),
         repeated: Default::default(),
```

### Comparing `slint-1.6.0a6/internal/compiler/passes/flickable.rs` & `slint-1.6.0a7/internal/compiler/passes/flickable.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/passes/focus_handling.rs` & `slint-1.6.0a7/internal/compiler/passes/focus_handling.rs`

 * *Files 6% similar despite different names*

```diff
@@ -10,18 +10,21 @@
 use crate::diagnostics::{BuildDiagnostics, SourceLocation, Spanned};
 use crate::expression_tree::{BuiltinFunction, Expression};
 use crate::langtype::{ElementType, Type};
 use crate::namedreference::NamedReference;
 use crate::object_tree::*;
 use by_address::ByAddress;
 use std::collections::{HashMap, HashSet};
+use strum::IntoEnumIterator;
 
 /// Generate setup code to pass window focus to the root item or a forwarded focus if applicable.
 pub fn call_focus_on_init(component: &Rc<Component>) {
-    if let Some(focus_call_code) = call_focus_function(&component.root_element, None) {
+    if let Some(focus_call_code) =
+        call_set_focus_function(&component.root_element, None, FocusFunctionType::SetFocus)
+    {
         component.init_code.borrow_mut().focus_setting_code.push(focus_call_code);
     }
 }
 
 /// Remove any `forward-focus` bindings, resolve any local '.focus()' calls and create a 'focus()'
 /// function on the root element if necessary.
 pub fn replace_forward_focus_bindings_with_focus_functions(
@@ -31,37 +34,40 @@
     for component in doc.inner_components.iter() {
         // Phase 1: Collect all forward-forward bindings
         let mut local_forwards = LocalFocusForwards::collect(component, diag);
 
         // Phase 2: Filter out focus-forward bindings that aren't callable
         local_forwards.remove_uncallable_forwards();
 
-        // Phase 3: For `focus-forward` in the root element, create a `focus()` function that's callable from the outside
+        // Phase 3: For `focus-forward` in the root element, create `focus()` and `clear-focus()` functions that are callable from the outside
         if let Some((root_focus_forward, focus_forward_location)) =
             local_forwards.focus_forward_for_element(&component.root_element)
         {
-            if let Some(set_focus_code) =
-                call_focus_function(&root_focus_forward, Some(&focus_forward_location))
-            {
-                component.root_element.borrow_mut().property_declarations.insert(
-                    "focus".into(),
-                    PropertyDeclaration {
-                        property_type: Type::Function {
-                            return_type: Type::Void.into(),
-                            args: vec![],
+            for function in FocusFunctionType::iter() {
+                if let Some(set_or_clear_focus_code) = call_set_focus_function(
+                    &root_focus_forward,
+                    Some(&focus_forward_location),
+                    function,
+                ) {
+                    component.root_element.borrow_mut().property_declarations.insert(
+                        function.name().into(),
+                        PropertyDeclaration {
+                            property_type: Type::Function {
+                                return_type: Type::Void.into(),
+                                args: vec![],
+                            },
+                            visibility: PropertyVisibility::Public,
+                            ..Default::default()
                         },
-                        visibility: PropertyVisibility::Public,
-                        ..Default::default()
-                    },
-                );
-                component
-                    .root_element
-                    .borrow_mut()
-                    .bindings
-                    .insert("focus".into(), RefCell::new(set_focus_code.into()));
+                    );
+                    component.root_element.borrow_mut().bindings.insert(
+                        function.name().into(),
+                        RefCell::new(set_or_clear_focus_code.into()),
+                    );
+                }
             }
         }
 
         // Phase 4: All calls to `.focus()` may need to be changed with `focus-forward` resolved or changed from the built-in
         // SetFocusItem() call to a regular function call to the component's focus() function.
         visit_all_expressions(component, |e, _| {
             local_forwards.resolve_focus_calls_in_expression(e)
@@ -119,15 +125,15 @@
 
         Self { forwards, diag }
     }
 
     fn remove_uncallable_forwards(&mut self) {
         for target_and_location in self.forwards.values_mut() {
             let (target, source_location) = target_and_location.as_ref().unwrap();
-            if call_focus_function(target, None).is_none() {
+            if call_set_focus_function(target, None, FocusFunctionType::SetFocus).is_none() {
                 self.diag.push_error(
                     "Cannot forward focus to unfocusable element".into(),
                     source_location,
                 );
                 *target_and_location = None;
             }
         }
@@ -157,67 +163,102 @@
             }
         }
     }
 
     fn resolve_focus_calls_in_expression(&mut self, expr: &mut Expression) {
         expr.visit_mut(|e| self.resolve_focus_calls_in_expression(e));
 
-        if let Expression::FunctionCall { function, arguments, .. } = expr {
-            if let Expression::BuiltinFunctionReference(
-                BuiltinFunction::SetFocusItem,
-                source_location,
-            ) = function.as_ref()
-            {
-                if arguments.len() != 1 {
-                    assert!(
-                        self.diag.has_error(),
-                        "Invalid argument generated for SetFocusItem call"
-                    );
-                    return;
-                }
-                if let Expression::ElementReference(weak_focus_target) = &arguments[0] {
-                    let mut focus_target = weak_focus_target.upgrade().expect(
-                        "internal compiler error: weak SetFocusItem parameter cannot be dangling",
-                    );
-
-                    if self.forwards.contains_key(&ByAddress(focus_target.clone())) {
-                        let Some((next_focus_target, _)) =
-                            self.focus_forward_for_element(&focus_target)
-                        else {
-                            // There's no need to report an additional error that focus() can't be called. Invalid
-                            // forward-focus bindings have already diagnostics produced for them.
-                            return;
-                        };
-                        focus_target = next_focus_target;
+        for focus_function in FocusFunctionType::iter() {
+            if let Expression::FunctionCall { function, arguments, .. } = expr {
+                if let Expression::BuiltinFunctionReference(
+                    builtin_function_type,
+                    source_location,
+                ) = function.as_ref()
+                {
+                    if *builtin_function_type != focus_function.as_builtin_function() {
+                        continue;
                     }
-
-                    if let Some(set_focus_code) =
-                        call_focus_function(&focus_target, source_location.as_ref())
-                    {
-                        *expr = set_focus_code;
-                    } else {
-                        self.diag.push_error(
-                            "focus() can only be called on focusable elements".into(),
-                            source_location,
+                    if arguments.len() != 1 {
+                        assert!(
+                            self.diag.has_error(),
+                            "Invalid argument generated for {} call",
+                            focus_function.name()
                         );
+                        return;
+                    }
+                    if let Expression::ElementReference(weak_focus_target) = &arguments[0] {
+                        let mut focus_target = weak_focus_target.upgrade().expect(
+                            "internal compiler error: weak focus/clear-focus parameter cannot be dangling"
+                        );
+
+                        if self.forwards.contains_key(&ByAddress(focus_target.clone())) {
+                            let Some((next_focus_target, _)) =
+                                self.focus_forward_for_element(&focus_target)
+                            else {
+                                // There's no need to report an additional error that focus() can't be called. Invalid
+                                // forward-focus bindings have already diagnostics produced for them.
+                                return;
+                            };
+                            focus_target = next_focus_target;
+                        }
+
+                        if let Some(set_or_clear_focus_code) = call_set_focus_function(
+                            &focus_target,
+                            source_location.as_ref(),
+                            focus_function,
+                        ) {
+                            *expr = set_or_clear_focus_code;
+                        } else {
+                            self.diag.push_error(
+                                format!(
+                                    "{}() can only be called on focusable elements",
+                                    focus_function.name(),
+                                ),
+                                source_location,
+                            );
+                        }
                     }
                 }
             }
         }
     }
 }
 
-fn call_focus_function(
+#[derive(Copy, Clone, strum::EnumIter)]
+enum FocusFunctionType {
+    SetFocus,
+    ClearFocus,
+}
+
+impl FocusFunctionType {
+    fn name(&self) -> &'static str {
+        match self {
+            Self::SetFocus => "focus",
+            Self::ClearFocus => "clear-focus",
+        }
+    }
+
+    fn as_builtin_function(&self) -> BuiltinFunction {
+        match self {
+            Self::SetFocus => BuiltinFunction::SetFocusItem,
+            Self::ClearFocus => BuiltinFunction::ClearFocusItem,
+        }
+    }
+}
+
+fn call_set_focus_function(
     element: &ElementRc,
     source_location: Option<&SourceLocation>,
+    function_type: FocusFunctionType,
 ) -> Option<Expression> {
+    let function_name = function_type.name();
     let declares_focus_function = {
         let mut element = element.clone();
         loop {
-            if element.borrow().property_declarations.contains_key("focus") {
+            if element.borrow().property_declarations.contains_key(function_name) {
                 break true;
             }
             let base = element.borrow().base_type.clone();
             match base {
                 ElementType::Component(compo) => element = compo.root_element.clone(),
                 _ => break false,
             }
@@ -225,25 +266,25 @@
     };
     let builtin_focus_function =
         element.borrow().builtin_type().map_or(false, |ty| ty.accepts_focus);
 
     if declares_focus_function {
         Some(Expression::FunctionCall {
             function: Box::new(Expression::FunctionReference(
-                NamedReference::new(element, "focus"),
+                NamedReference::new(element, function_name),
                 None,
             )),
             arguments: vec![],
             source_location: source_location.cloned(),
         })
     } else if builtin_focus_function {
         let source_location = source_location.cloned();
         Some(Expression::FunctionCall {
             function: Box::new(Expression::BuiltinFunctionReference(
-                BuiltinFunction::SetFocusItem,
+                function_type.as_builtin_function(),
                 source_location.clone(),
             )),
             arguments: vec![Expression::ElementReference(Rc::downgrade(element))],
             source_location,
         })
     } else {
         None
```

### Comparing `slint-1.6.0a6/internal/compiler/passes/generate_item_indices.rs` & `slint-1.6.0a7/internal/compiler/passes/generate_item_indices.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/passes/infer_aliases_types.rs` & `slint-1.6.0a7/internal/compiler/passes/infer_aliases_types.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/passes/inlining.rs` & `slint-1.6.0a7/internal/compiler/passes/inlining.rs`

 * *Files 3% similar despite different names*

```diff
@@ -50,19 +50,17 @@
             .popup_windows
             .borrow()
             .iter()
             .for_each(|p| inline_components_recursively(&p.component, inline_selection))
     }
     inline_components_recursively(&doc.root_component, inline_selection);
 
-    if matches!(inline_selection, InlineSelection::InlineAllComponents) {
-        let mut init_code = doc.root_component.init_code.borrow_mut();
-        let inlined_init_code = core::mem::take(&mut init_code.inlined_init_code);
-        init_code.constructor_code.splice(0..0, inlined_init_code.into_values());
-    }
+    let mut init_code = doc.root_component.init_code.borrow_mut();
+    let inlined_init_code = core::mem::take(&mut init_code.inlined_init_code);
+    init_code.constructor_code.splice(0..0, inlined_init_code.into_values());
 }
 
 fn clone_tuple<U: Clone, V: Clone>((u, v): (&U, &V)) -> (U, V) {
     (u.clone(), v.clone())
 }
 
 fn element_key(e: ElementRc) -> ByAddress<ElementRc> {
@@ -151,40 +149,38 @@
         inlined_component
             .popup_windows
             .borrow()
             .iter()
             .map(|p| duplicate_popup(p, &mut mapping, priority_delta)),
     );
 
-    // When inlining a component before the collect_init_code phase, do the collect_init_code phase for
-    // the init callback in the inlined component manually, by cloning the expression into the init_code
-    // and skipping "init" in the binding merge phase.
-    let maybe_init_callback_to_inline = inlined_component
-        .root_element
-        .borrow()
-        .bindings
-        .get("init")
-        .map(|binding| binding.borrow().expression.clone());
-
-    for (k, val) in
-        inlined_component.root_element.borrow().bindings.iter().filter(|(k, _)| *k != "init")
-    {
+    for (k, val) in inlined_component.root_element.borrow().bindings.iter() {
         match elem_mut.bindings.entry(k.clone()) {
             std::collections::btree_map::Entry::Vacant(entry) => {
                 let priority = &mut entry.insert(val.clone()).get_mut().priority;
                 *priority = priority.saturating_add(priority_delta);
             }
             std::collections::btree_map::Entry::Occupied(mut entry) => {
                 let entry = entry.get_mut().get_mut();
                 if entry.merge_with(&val.borrow()) {
                     entry.priority = entry.priority.saturating_add(priority_delta);
                 }
             }
         }
     }
+    for (k, val) in inlined_component.root_element.borrow().change_callbacks.iter() {
+        match elem_mut.change_callbacks.entry(k.clone()) {
+            std::collections::btree_map::Entry::Vacant(entry) => {
+                entry.insert(val.clone());
+            }
+            std::collections::btree_map::Entry::Occupied(mut entry) => {
+                entry.get_mut().get_mut().extend_from_slice(&*val.borrow());
+            }
+        }
+    }
 
     if let Some(orig) = &inlined_component.root_element.borrow().layout_info_prop {
         if let Some(_new) = &mut elem_mut.layout_info_prop {
             todo!("Merge layout infos");
         } else {
             elem_mut.layout_info_prop = Some(orig.clone());
         }
@@ -196,21 +192,14 @@
         // Fix up any property references from within already collected init code.
         visit_named_references_in_expression(&mut init_code, &mut |nr| {
             fixup_reference(nr, &mapping)
         });
         fixup_element_references(&mut init_code, &mapping);
         init_code
     };
-
-    root_component
-        .init_code
-        .borrow_mut()
-        .constructor_code
-        .extend(maybe_init_callback_to_inline.map(fixup_init_expression));
-
     let inlined_init_code = inlined_component
         .init_code
         .borrow()
         .inlined_init_code
         .values()
         .cloned()
         .chain(
@@ -255,14 +244,15 @@
         property_declarations: elem.property_declarations.clone(),
         // We will do the fixup of the references in bindings later
         bindings: elem
             .bindings
             .iter()
             .map(|b| duplicate_binding(b, mapping, root_component, priority_delta))
             .collect(),
+        change_callbacks: elem.change_callbacks.clone(),
         property_analysis: elem.property_analysis.clone(),
         children: elem
             .children
             .iter()
             .map(|x| duplicate_element_with_mapping(x, mapping, root_component, priority_delta))
             .collect(),
         repeated: elem.repeated.clone(),
```

### Comparing `slint-1.6.0a6/internal/compiler/passes/lower_absolute_coordinates.rs` & `slint-1.6.0a7/internal/compiler/passes/lower_absolute_coordinates.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/passes/lower_accessibility.rs` & `slint-1.6.0a7/internal/compiler/passes/lower_accessibility.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/passes/lower_component_container.rs` & `slint-1.6.0a7/internal/compiler/passes/lower_component_container.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/passes/lower_layout.rs` & `slint-1.6.0a7/internal/compiler/passes/lower_layout.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/passes/lower_popups.rs` & `slint-1.6.0a7/internal/compiler/passes/lower_popups.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/passes/lower_property_to_element.rs` & `slint-1.6.0a7/internal/compiler/passes/lower_property_to_element.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/passes/lower_shadows.rs` & `slint-1.6.0a7/internal/compiler/passes/lower_shadows.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/passes/lower_states.rs` & `slint-1.6.0a7/internal/compiler/passes/lower_states.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/passes/lower_tabwidget.rs` & `slint-1.6.0a7/internal/compiler/passes/lower_tabwidget.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/passes/lower_text_input_interface.rs` & `slint-1.6.0a7/internal/compiler/passes/lower_text_input_interface.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/passes/materialize_fake_properties.rs` & `slint-1.6.0a7/internal/compiler/passes/materialize_fake_properties.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/passes/move_declarations.rs` & `slint-1.6.0a7/internal/compiler/passes/move_declarations.rs`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 // Copyright © SixtyFPS GmbH <info@slint.dev>
 // SPDX-License-Identifier: GPL-3.0-only OR LicenseRef-Slint-Royalty-free-1.2 OR LicenseRef-Slint-commercial
 
 //! This pass moves all declaration of properties or callback to the root
 
-use crate::expression_tree::NamedReference;
-use crate::object_tree::*;
-
+use crate::expression_tree::{Expression, NamedReference};
 use crate::langtype::ElementType;
-use std::collections::BTreeMap;
-use std::collections::HashMap;
+use crate::object_tree::*;
+use core::cell::RefCell;
+use std::collections::{BTreeMap, HashMap};
 use std::rc::Rc;
 
 struct Declarations {
     property_declarations: BTreeMap<String, PropertyDeclaration>,
 }
 impl Declarations {
     fn take_from_element(e: &mut Element) -> Self {
@@ -26,14 +25,15 @@
 }
 
 fn do_move_declarations(component: &Rc<Component>) {
     let mut decl = Declarations::take_from_element(&mut component.root_element.borrow_mut());
     component.popup_windows.borrow().iter().for_each(|f| do_move_declarations(&f.component));
 
     let mut new_root_bindings = HashMap::new();
+    let mut new_root_change_callbacks = HashMap::new();
     let mut new_root_property_analysis = HashMap::new();
 
     let move_bindings_and_animations = &mut |elem: &ElementRc| {
         visit_all_named_references_in_element(elem, fixup_reference);
 
         if elem.borrow().repeated.is_some() {
             if let ElementType::Component(base) = &elem.borrow().base_type {
@@ -68,14 +68,27 @@
             if will_be_moved {
                 new_root_property_analysis.insert(map_name(elem, prop.as_str()), a);
             } else {
                 new_property_analysis.insert(prop, a);
             }
         }
         *elem.borrow().property_analysis.borrow_mut() = new_property_analysis;
+
+        // Also move the changed callback
+        let change_callbacks = core::mem::take(&mut elem.borrow_mut().change_callbacks);
+        let mut new_change_callbacks = BTreeMap::<String, RefCell<Vec<Expression>>>::default();
+        for (k, e) in change_callbacks {
+            let will_be_moved = elem.borrow().property_declarations.contains_key(&k);
+            if will_be_moved {
+                new_root_change_callbacks.insert(map_name(elem, k.as_str()), e);
+            } else {
+                new_change_callbacks.insert(k, e);
+            }
+        }
+        elem.borrow_mut().change_callbacks = new_change_callbacks;
     };
 
     component.optimized_elements.borrow().iter().for_each(|e| move_bindings_and_animations(e));
     recurse_elem(&component.root_element, &(), &mut |e, _| move_bindings_and_animations(e));
 
     component.root_constraints.borrow_mut().visit_named_references(&mut fixup_reference);
     component.popup_windows.borrow_mut().iter_mut().for_each(|p| {
@@ -102,14 +115,15 @@
     component.optimized_elements.borrow().iter().for_each(move_properties);
 
     {
         let mut r = component.root_element.borrow_mut();
         r.property_declarations = decl.property_declarations;
         r.bindings.extend(new_root_bindings);
         r.property_analysis.borrow_mut().extend(new_root_property_analysis);
+        r.change_callbacks.extend(new_root_change_callbacks);
     }
 }
 
 fn fixup_reference(nr: &mut NamedReference) {
     let e = nr.element();
     let component = e.borrow().enclosing_component.upgrade().unwrap();
     if !Rc::ptr_eq(&e, &component.root_element)
```

### Comparing `slint-1.6.0a6/internal/compiler/passes/optimize_useless_rectangles.rs` & `slint-1.6.0a7/internal/compiler/passes/optimize_useless_rectangles.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/passes/purity_check.rs` & `slint-1.6.0a7/internal/compiler/passes/purity_check.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/passes/remove_aliases.rs` & `slint-1.6.0a7/internal/compiler/passes/remove_aliases.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/passes/remove_return.rs` & `slint-1.6.0a7/internal/compiler/passes/remove_return.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/passes/remove_unused_properties.rs` & `slint-1.6.0a7/internal/compiler/passes/remove_unused_properties.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/passes/repeater_component.rs` & `slint-1.6.0a7/internal/compiler/passes/repeater_component.rs`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,15 @@
         let mut elem = elem.borrow_mut();
 
         let comp = Rc::new(Component {
             root_element: Rc::new(RefCell::new(Element {
                 id: elem.id.clone(),
                 base_type: std::mem::take(&mut elem.base_type),
                 bindings: std::mem::take(&mut elem.bindings),
+                change_callbacks: std::mem::take(&mut elem.change_callbacks),
                 property_analysis: std::mem::take(&mut elem.property_analysis),
                 children: std::mem::take(&mut elem.children),
                 property_declarations: std::mem::take(&mut elem.property_declarations),
                 named_references: Default::default(),
                 repeated: None,
                 is_component_placeholder: false,
                 debug: elem.debug.clone(),
```

### Comparing `slint-1.6.0a6/internal/compiler/passes/resolve_native_classes.rs` & `slint-1.6.0a7/internal/compiler/passes/resolve_native_classes.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/passes/resolving.rs` & `slint-1.6.0a7/internal/compiler/passes/resolving.rs`

 * *Files 0% similar despite different names*

```diff
@@ -43,26 +43,29 @@
             type_register,
             type_loader: Some(type_loader),
             current_token: None,
         };
 
         let new_expr = match node.kind() {
             SyntaxKind::CallbackConnection => {
-                //FIXME: proper callback support (node is a codeblock)
                 Expression::from_callback_connection(node.clone().into(), &mut lookup_ctx)
             }
             SyntaxKind::Function => Expression::from_function(node.clone().into(), &mut lookup_ctx),
             SyntaxKind::Expression => {
                 //FIXME again: this happen for non-binding expression (i.e: model)
                 Expression::from_expression_node(node.clone().into(), &mut lookup_ctx)
                     .maybe_convert_to(lookup_ctx.property_type.clone(), node, diag)
             }
             SyntaxKind::BindingExpression => {
                 Expression::from_binding_expression_node(node.clone(), &mut lookup_ctx)
             }
+            SyntaxKind::PropertyChangedCallback => Expression::from_codeblock_node(
+                syntax_nodes::PropertyChangedCallback::from(node.clone()).CodeBlock(),
+                &mut lookup_ctx,
+            ),
             SyntaxKind::TwoWayBinding => {
                 assert!(diag.has_error(), "Two way binding should have been resolved already  (property: {property_name:?})");
                 Expression::Invalid
             }
             _ => {
                 debug_assert!(diag.has_error());
                 Expression::Invalid
```

### Comparing `slint-1.6.0a6/internal/compiler/passes/unique_id.rs` & `slint-1.6.0a7/internal/compiler/passes/unique_id.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/passes/visible.rs` & `slint-1.6.0a7/internal/compiler/passes/visible.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/passes/z_order.rs` & `slint-1.6.0a7/internal/compiler/passes/z_order.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/passes.rs` & `slint-1.6.0a7/internal/compiler/passes.rs`

 * *Files 2% similar despite different names*

```diff
@@ -88,37 +88,45 @@
         compile_paths::compile_paths(
             component,
             &doc.local_registry,
             type_loader.compiler_config.embed_resources,
             diag,
         );
         lower_tabwidget::lower_tabwidget(component, type_loader, diag).await;
+    }
+
+    collect_subcomponents::collect_subcomponents(root_component);
+
+    for component in (root_component.used_types.borrow().sub_components.iter())
+        .chain(std::iter::once(root_component))
+    {
         apply_default_properties_from_style::apply_default_properties_from_style(
             component,
             &style_metrics,
             diag,
         );
         lower_states::lower_states(component, &doc.local_registry, diag);
         lower_text_input_interface::lower_text_input_interface(component);
+        repeater_component::process_repeater_components(component);
+        lower_popups::lower_popups(component, &doc.local_registry, diag);
+        collect_init_code::collect_init_code(component);
     }
 
     inlining::inline(doc, inlining::InlineSelection::InlineOnlyRequiredComponents);
     collect_subcomponents::collect_subcomponents(root_component);
 
     focus_handling::call_focus_on_init(root_component);
 
     ensure_window::ensure_window(root_component, &doc.local_registry, &style_metrics);
 
     for component in (root_component.used_types.borrow().sub_components.iter())
         .chain(std::iter::once(root_component))
     {
         border_radius::handle_border_radius(component, diag);
         flickable::handle_flickable(component, &global_type_registry.borrow());
-        repeater_component::process_repeater_components(component);
-        lower_popups::lower_popups(component, &doc.local_registry, diag);
         lower_component_container::lower_component_container(component, &doc.local_registry, diag);
 
         lower_layout::lower_layouts(component, type_loader, diag).await;
         default_geometry::default_geometry(component, diag);
         lower_absolute_coordinates::lower_absolute_coordinates(component);
         z_order::reorder_by_z_order(component, diag);
         lower_property_to_element::lower_property_to_element(
@@ -165,15 +173,14 @@
             &global_type_registry.borrow(),
             diag,
         );
         clip::handle_clip(component, &global_type_registry.borrow(), diag);
         if type_loader.compiler_config.accessibility {
             lower_accessibility::lower_accessibility_properties(component, diag);
         }
-        collect_init_code::collect_init_code(component);
         materialize_fake_properties::materialize_fake_properties(component);
     }
     lower_layout::check_window_layout(root_component);
     collect_globals::collect_globals(doc, diag);
 
     if type_loader.compiler_config.inline_all_elements {
         inlining::inline(doc, inlining::InlineSelection::InlineAllComponents);
```

### Comparing `slint-1.6.0a6/internal/compiler/pathutils.rs` & `slint-1.6.0a7/internal/compiler/pathutils.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/consistent_styles.rs` & `slint-1.6.0a7/internal/compiler/tests/consistent_styles.rs`

 * *Files 2% similar despite different names*

```diff
@@ -88,24 +88,32 @@
                                 ty: v.ty.clone(),
                                 vis: v.property_visibility,
                                 pure: false,
                             },
                         )
                     }),
                 );
-                // Synthesize focus() as styles written in .slint will have it but the qt style exposes NativeXX directly.
+                // Synthesize focus() and `clear-focus()` as styles written in .slint will have it but the qt style exposes NativeXX directly.
                 if b.accepts_focus {
                     result.properties.insert(
                         "focus".into(),
                         PropertyInfo {
                             ty: Type::Function { return_type: Type::Void.into(), args: vec![] },
                             vis: PropertyVisibility::Public,
                             pure: false,
                         },
                     );
+                    result.properties.insert(
+                        "clear-focus".into(),
+                        PropertyInfo {
+                            ty: Type::Function { return_type: Type::Void.into(), args: vec![] },
+                            vis: PropertyVisibility::Public,
+                            pure: false,
+                        },
+                    );
                 }
                 break;
             }
             i_slint_compiler::langtype::ElementType::Native(_) => unreachable!(),
             i_slint_compiler::langtype::ElementType::Error => unreachable!(),
             i_slint_compiler::langtype::ElementType::Global => break,
         };
```

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/accessibility/accessible_properties.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/accessibility/accessible_properties.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/analysis/binding_loop1.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/analysis/binding_loop1.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/analysis/binding_loop2.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/analysis/binding_loop2.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/analysis/binding_loop_function.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/analysis/binding_loop_function.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/analysis/binding_loop_issue_772.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/analysis/binding_loop_issue_772.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/analysis/binding_loop_layout.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/analysis/binding_loop_layout.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/analysis/binding_loop_layout2.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/analysis/binding_loop_layout2.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/analysis/binding_loop_layout3.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/analysis/binding_loop_layout3.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/analysis/binding_loop_layout4.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/analysis/binding_loop_layout4.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/analysis/binding_loop_self.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/analysis/binding_loop_self.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/basic/animate.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/basic/animate.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/basic/assign.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/basic/assign.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/basic/box_shadow.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/basic/box_shadow.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/basic/children_placeholder.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/basic/children_placeholder.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/basic/clip.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/basic/clip.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/basic/dialog.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/basic/dialog.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/basic/dialog2.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/basic/dialog2.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/basic/duplicated_id.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/basic/duplicated_id.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/basic/easing.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/basic/easing.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/basic/enums.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/basic/enums.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/basic/item_as_property.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/basic/item_as_property.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/basic/layout2.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/basic/layout2.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/basic/linear-gradient.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/basic/linear-gradient.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/basic/opacity.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/basic/opacity.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/basic/parse_error.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/basic/parse_error.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/basic/path.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/basic/path.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/basic/path_commands.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/basic/path_commands.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/basic/path_for.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/basic/path_for.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/basic/percent.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/basic/percent.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/basic/popup.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/basic/popup.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/basic/property_declaration.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/basic/property_declaration.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/basic/radial-gradient.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/basic/radial-gradient.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/basic/return.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/basic/return.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/basic/rotation.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/basic/rotation.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/basic/self_assign.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/basic/self_assign.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/basic/signal.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/basic/signal.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/basic/states_transitions.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/basic/states_transitions.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/basic/states_transitions2.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/basic/states_transitions2.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/basic/states_transitions3.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/basic/states_transitions3.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/basic/states_two_way.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/basic/states_two_way.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/basic/sub_elements.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/basic/sub_elements.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/basic/tr.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/basic/tr.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/basic/tr2.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/basic/tr2.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/basic/type_declaration.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/basic/type_declaration.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/basic/unknown_item.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/basic/unknown_item.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/elements/component_container.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/elements/component_container.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/elements/listview.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/elements/listview.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/elements/popup.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/elements/popup.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/elements/tabwidget.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/elements/tabwidget.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/elements/tabwidget2.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/elements/tabwidget2.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/exports/reexport_duplicate.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/exports/reexport_duplicate.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/expressions/arithmetic_op.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/expressions/arithmetic_op.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/expressions/clamp.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/expressions/clamp.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/expressions/comparison_operator.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/expressions/comparison_operator.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/expressions/condition_operator.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/expressions/condition_operator.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/expressions/image-url.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/expressions/image-url.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/expressions/image-url2.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/expressions/image-url2.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/expressions/minmax.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/expressions/minmax.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/expressions/percent2.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/expressions/percent2.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/expressions/unary_op.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/expressions/unary_op.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/focus/focus_not_called.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/focus/focus_not_called.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/focus/focus_wrong_args.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/focus/focus_wrong_args.slint`

 * *Files 24% similar despite different names*

```diff
@@ -11,12 +11,14 @@
         clicked => {
             fs.focus(0);
 //          ^error{The callback or function expects 0 arguments, but 1 are provided}
             ta.focus();
 //             ^error{focus\(\) can only be called on focusable elements}
             ta.focus(0);
 //          ^error{The callback or function expects 0 arguments, but 1 are provided}
+            ta.clear-focus();
+//             ^error{clear-focus\(\) can only be called on focusable elements}
         }
     }
 
 
 }
```

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/focus/initial_focus_non_input.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/focus/initial_focus_non_input.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/functions/function_double_qualified.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/functions/function_double_qualified.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/functions/functions.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/functions/functions.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/functions/functions_call.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/functions/functions_call.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/functions/functions_purity.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/functions/functions_purity.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/imports/bug_2719.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/imports/bug_2719.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/imports/bug_3674_alias-from-broken-import.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/imports/bug_3674_alias-from-broken-import.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/imports/import_errors.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/imports/import_errors.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/layout/if_in_grid.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/layout/if_in_grid.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/layout/min_max_conflict.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/layout/min_max_conflict.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/layout/spacing.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/layout/spacing.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/lookup/array_index.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/lookup/array_index.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/lookup/callback_alias.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/lookup/callback_alias.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/lookup/callback_alias2.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/lookup/callback_alias2.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/lookup/callback_alias3.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/lookup/callback_alias3.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/lookup/color.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/lookup/color.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/lookup/conversion.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/lookup/conversion.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/lookup/dashes.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/lookup/dashes.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/lookup/deprecated_property.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/lookup/deprecated_property.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/lookup/enum.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/lookup/enum.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/lookup/for_lookup.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/lookup/for_lookup.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/lookup/global.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/lookup/global.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/lookup/if.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/lookup/if.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/lookup/issue_1461.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/lookup/issue_1461.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/lookup/property.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/lookup/property.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/lookup/recover_id_lookup.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/lookup/recover_id_lookup.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/lookup/signal_arg.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/lookup/signal_arg.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/lookup/two_way_binding.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/lookup/two_way_binding.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/lookup/two_way_binding_infer.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/lookup/two_way_binding_infer.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/new_syntax/deprecated_syntax.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/new_syntax/deprecated_syntax.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/new_syntax/input_output.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/new_syntax/input_output.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/new_syntax/input_output2.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/new_syntax/input_output2.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/new_syntax/new_component.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/new_syntax/new_component.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/new_syntax/new_lookup.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/new_syntax/new_lookup.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/new_syntax/two_way_input_output.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/new_syntax/two_way_input_output.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/parse_error/property2.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/parse_error/property2.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/parse_error/state1.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/parse_error/state1.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax/parse_error/struct.slint` & `slint-1.6.0a7/internal/compiler/tests/syntax/parse_error/struct.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/tests/syntax_tests.rs` & `slint-1.6.0a7/internal/compiler/tests/syntax_tests.rs`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,15 @@
     let syntax_node =
         i_slint_compiler::parser::parse(source.clone(), Some(path), None, &mut parse_diagnostics);
 
     let has_parse_error = parse_diagnostics.has_error();
     let mut compiler_config = i_slint_compiler::CompilerConfiguration::new(
         i_slint_compiler::generator::OutputFormat::Interpreter,
     );
-    compiler_config.enable_component_containers = true;
+    compiler_config.enable_experimental = true;
     compiler_config.style = Some("fluent".into());
     let compile_diagnostics = if !parse_diagnostics.has_error() {
         let (_, build_diags, _) = spin_on::spin_on(i_slint_compiler::compile_syntax_node(
             syntax_node.clone(),
             parse_diagnostics,
             compiler_config.clone(),
         ));
```

### Comparing `slint-1.6.0a6/internal/compiler/typeloader.rs` & `slint-1.6.0a7/internal/compiler/typeloader.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/typeregister.rs` & `slint-1.6.0a7/internal/compiler/typeregister.rs`

 * *Files 2% similar despite different names*

```diff
@@ -136,14 +136,15 @@
                 .iter()
                 .map(|(k, v)| (*k, v.clone(), PropertyVisibility::Constexpr)),
         )
         .chain(IntoIterator::into_iter([
             ("absolute-position", logical_point_type(), PropertyVisibility::Output),
             ("forward-focus", Type::ElementReference, PropertyVisibility::Constexpr),
             ("focus", BuiltinFunction::SetFocusItem.ty(), PropertyVisibility::Public),
+            ("clear-focus", BuiltinFunction::ClearFocusItem.ty(), PropertyVisibility::Public),
             (
                 "dialog-button-role",
                 Type::Enumeration(BUILTIN_ENUMS.with(|e| e.DialogButtonRole.clone())),
                 PropertyVisibility::Constexpr,
             ),
             (
                 "accessible-role",
@@ -202,14 +203,15 @@
     }
 }
 
 /// These member functions are injected in every time
 pub fn reserved_member_function(name: &str) -> Option<BuiltinFunction> {
     for (m, e) in [
         ("focus", BuiltinFunction::SetFocusItem), // match for callable "focus" property
+        ("clear-focus", BuiltinFunction::ClearFocusItem), // match for callable "clear-focus" property
     ] {
         if m == name {
             return Some(e);
         }
     }
     None
 }
```

### Comparing `slint-1.6.0a6/internal/compiler/widgets/common/MadeWithSlint-logo-dark.svg` & `slint-1.6.0a7/internal/compiler/widgets/common/MadeWithSlint-logo-dark.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/common/MadeWithSlint-logo-light.svg` & `slint-1.6.0a7/internal/compiler/widgets/common/MadeWithSlint-logo-light.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/common/combobox-base.slint` & `slint-1.6.0a7/internal/compiler/widgets/common/combobox-base.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/common/common.slint` & `slint-1.6.0a7/internal/compiler/widgets/common/common.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/common/lineedit-base.slint` & `slint-1.6.0a7/internal/compiler/widgets/common/lineedit-base.slint`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,16 @@
         text: (root.text == "" && i-text-input.preedit-text == "") ? root.placeholder-text : "";
         font-size:  i-text-input.font-size;
         font-italic: i-text-input.font-italic;
         font-weight: i-text-input.font-weight;
         font-family: i-text-input.font-family;
         color: root.placeholder-color;
         horizontal-alignment: root.horizontal-alignment;
+        // the label is set on the LineEdit itself
+        accessible-role: none;
     }
 
     i-text-input := TextInput {
         property <length> computed-x;
 
         x: min(0px, max(parent.width - self.width - self.text-cursor-width, self.computed-x));
         width: max(parent.width - self.text-cursor-width, self.preferred-width);
```

### Comparing `slint-1.6.0a6/internal/compiler/widgets/common/listview.slint` & `slint-1.6.0a7/internal/compiler/widgets/common/listview.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/common/slider-base.slint` & `slint-1.6.0a7/internal/compiler/widgets/common/slider-base.slint`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     out property <bool> pressed <=> touch-area.enabled;
     out property <bool> has-hover <=> touch-area.has-hover;
     out property <bool> vertical: root.orientation == Orientation.vertical;
     out property <bool> has-focus <=> focus-scope.has-focus;
     out property <bool> handle-has-hover: touch-area.mouse-x >= root.handle-x && touch-area.mouse-x <= root.handle-x + root.handle-width &&
         touch-area.mouse-y >= root.handle-y && touch-area.mouse-y <= root.handle-y + root.handle-height;
     out property <bool> handle-pressed;
-    in-out property <float> value: 0;
+    in-out property <float> value: minimum;
 
     callback changed(/* value */ float);
     callback released(/* value */ float);
 
     private property <length> ref-size: !root.vertical ? root.handle-width : root.handle-height;
 
     forward-focus: focus-scope;
```

### Comparing `slint-1.6.0a6/internal/compiler/widgets/common/spinbox-base.slint` & `slint-1.6.0a7/internal/compiler/widgets/common/spinbox-base.slint`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     in property <brush> color <=> i-text-input.color;
     in property <length> font-size <=> i-text-input.font-size;
     in property <int> font-weight <=> i-text-input.font-weight;
     in property <color> selection-background-color <=> i-text-input.selection-background-color;
     in property <color> selection-foreground-color <=> i-text-input.selection-foreground-color;
     in property <TextHorizontalAlignment> horizontal-alignment <=> i-text-input.horizontal-alignment;
     out property <bool> has-focus <=> i-text-input.has-focus;
-    in-out property <int> value;
+    in-out property <int> value: minimum;
 
     callback edited(/* value */ int);
 
     public function update-value(value: int) {
         if (value >= root.minimum && value <= root.maximum) {
             root.value = value;
             root.edited(value);
```

### Comparing `slint-1.6.0a6/internal/compiler/widgets/common/spinner-base.slint` & `slint-1.6.0a7/internal/compiler/widgets/common/spinner-base.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/common/standardbutton.slint` & `slint-1.6.0a7/internal/compiler/widgets/common/standardbutton.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/common/tabwidget-base.slint` & `slint-1.6.0a7/internal/compiler/widgets/common/tabwidget-base.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/cosmic-base/button.slint` & `slint-1.6.0a7/internal/compiler/widgets/cosmic-base/button.slint`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     vertical-stretch: 0;
     forward-focus: state-layer;
 
     accessible-role: button;
     accessible-checkable: root.checkable;
     accessible-checked: root.checked;
     accessible-label: root.text;
-    accessible-action-default => { clicked(); }
+    accessible-action-default => { state-layer.clicked(); }
 
     states [
         disabled when !root.enabled : {
             root.opacity: 0.5;
         }
     ]
 
@@ -61,16 +61,16 @@
             if (root.text != ""): Text {
                 font-size: CosmicFontSettings.body.font-size;
                 font-weight: CosmicFontSettings.body.font-weight;
                 horizontal-alignment: center;
                 vertical-alignment: center;
                 text: root.text;
                 color: root.text-color;
-
                 animate color { duration: 150ms; }
+                accessible-role: none;
             }
         }
     }
 
     state-layer := StateLayer {
         border-radius: background.border-radius;
```

### Comparing `slint-1.6.0a6/internal/compiler/widgets/cosmic-base/checkbox.slint` & `slint-1.6.0a7/internal/compiler/widgets/cosmic-base/checkbox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/cosmic-base/combobox.slint` & `slint-1.6.0a7/internal/compiler/widgets/cosmic-base/combobox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/cosmic-base/components.slint` & `slint-1.6.0a7/internal/compiler/widgets/cosmic-base/components.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/cosmic-base/groupbox.slint` & `slint-1.6.0a7/internal/compiler/widgets/cosmic-base/groupbox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/cosmic-base/layouts.slint` & `slint-1.6.0a7/internal/compiler/widgets/cosmic-base/layouts.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/cosmic-base/lineedit.slint` & `slint-1.6.0a7/internal/compiler/widgets/cosmic-base/lineedit.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/cosmic-base/progressindicator.slint` & `slint-1.6.0a7/internal/compiler/widgets/cosmic-base/progressindicator.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/cosmic-base/scrollview.slint` & `slint-1.6.0a7/internal/compiler/widgets/cosmic-base/scrollview.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/cosmic-base/slider.slint` & `slint-1.6.0a7/internal/compiler/widgets/cosmic-base/slider.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/cosmic-base/spinbox.slint` & `slint-1.6.0a7/internal/compiler/widgets/cosmic-base/spinbox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/cosmic-base/spinner.slint` & `slint-1.6.0a7/internal/compiler/widgets/cosmic-base/spinner.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/cosmic-base/std-widgets-base.slint` & `slint-1.6.0a7/internal/compiler/widgets/cosmic-base/std-widgets-base.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/cosmic-base/std-widgets-impl.slint` & `slint-1.6.0a7/internal/compiler/widgets/cosmic-base/std-widgets-impl.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/cosmic-base/styling.slint` & `slint-1.6.0a7/internal/compiler/widgets/cosmic-base/styling.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/cosmic-base/switch.slint` & `slint-1.6.0a7/internal/compiler/widgets/cosmic-base/switch.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/cosmic-base/tableview.slint` & `slint-1.6.0a7/internal/compiler/widgets/cosmic-base/tableview.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/cosmic-base/tabwidget.slint` & `slint-1.6.0a7/internal/compiler/widgets/cosmic-base/tabwidget.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/cosmic-base/textedit.slint` & `slint-1.6.0a7/internal/compiler/widgets/cosmic-base/textedit.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/_arrow-down.svg` & `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/_arrow-down.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/_check-mark.svg` & `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/_check-mark.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/_chevron-down.svg` & `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/_chevron-down.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/_chevron-up.svg` & `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/_chevron-up.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/_down.svg` & `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/_down.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/_left.svg` & `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/_left.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/_right.svg` & `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/_right.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/_up.svg` & `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/_up.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/button.slint` & `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/button.slint`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     vertical-stretch: 0;
     forward-focus: i-focus-scope;
 
     accessible-role: button;
     accessible-checkable: root.checkable;
     accessible-checked: root.checked;
     accessible-label: root.text;
-    accessible-action-default => { clicked(); }
+    accessible-action-default => { i-touch-area.clicked(); }
 
 
     states [
         disabled when !i-touch-area.enabled : {
             root.text-color: CupertinoPalette.foreground-secondary;
             root.background: CupertinoPalette.quaternary-control-background;
         }
@@ -126,16 +126,16 @@
             opacity: root.enabled ? 1 : 0.5;
             font-size: CupertinoFontSettings.body.font-size;
             font-weight: CupertinoFontSettings.body.font-weight;
             horizontal-alignment: center;
             vertical-alignment: center;
             text: root.text;
             color: root.text-color;
-
             animate color { duration: 150ms; }
+            accessible-role: none;
         }
     }
 
     i-touch-area := TouchArea {
         clicked => {
             if (root.checkable) {
                 root.checked = !root.checked;
```

### Comparing `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/checkbox.slint` & `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/checkbox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/combobox.slint` & `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/combobox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/components.slint` & `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/components.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/groupbox.slint` & `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/groupbox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/layouts.slint` & `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/layouts.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/lineedit.slint` & `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/lineedit.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/progressindicator.slint` & `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/progressindicator.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/scrollview.slint` & `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/scrollview.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/slider.slint` & `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/slider.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/spinbox.slint` & `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/spinbox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/spinner.slint` & `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/spinner.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/std-widgets-base.slint` & `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/std-widgets-base.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/std-widgets-impl.slint` & `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/std-widgets-impl.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/styling.slint` & `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/styling.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/switch.slint` & `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/switch.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/tableview.slint` & `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/tableview.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/tabwidget.slint` & `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/tabwidget.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/cupertino-base/textedit.slint` & `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/textedit.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/fluent-base/_arrow-down.svg` & `slint-1.6.0a7/internal/compiler/widgets/fluent-base/_arrow-down.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/fluent-base/_check-mark.svg` & `slint-1.6.0a7/internal/compiler/widgets/fluent-base/_check-mark.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/fluent-base/_chevron-down.svg` & `slint-1.6.0a7/internal/compiler/widgets/fluent-base/_chevron-down.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/fluent-base/_chevron-up.svg` & `slint-1.6.0a7/internal/compiler/widgets/fluent-base/_chevron-up.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/fluent-base/_down.svg` & `slint-1.6.0a7/internal/compiler/widgets/fluent-base/_down.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/fluent-base/_left.svg` & `slint-1.6.0a7/internal/compiler/widgets/fluent-base/_left.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/fluent-base/_right.svg` & `slint-1.6.0a7/internal/compiler/widgets/fluent-base/_right.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/fluent-base/_up.svg` & `slint-1.6.0a7/internal/compiler/widgets/fluent-base/_up.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/fluent-base/button.slint` & `slint-1.6.0a7/internal/compiler/widgets/fluent-base/button.slint`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     vertical-stretch: 0;
     forward-focus: i-focus-scope;
 
     accessible-role: button;
     accessible-checkable: root.checkable;
     accessible-checked: root.checked;
     accessible-label: root.text;
-    accessible-action-default => { clicked(); }
+    accessible-action-default => { i-touch-area.clicked(); }
 
     states [
         disabled when !root.enabled : {
             i-background.background: root.primary || root.checked ? FluentPalette.accent-disabled : FluentPalette.control-disabled;
             i-border.border-color: root.primary || root.checked ? transparent : FluentPalette.border;
             root.text-color: root.primary || root.checked ? FluentPalette.text-accent-foreground-disabled : FluentPalette.text-disabled;
         }
@@ -82,16 +82,16 @@
             if (root.text != ""): Text {
                 font-size: FluentFontSettings.body.font-size;
                 font-weight: FluentFontSettings.body.font-weight;
                 horizontal-alignment: center;
                 vertical-alignment: center;
                 text: root.text;
                 color: root.text-color;
-
                 animate color { duration: 150ms; }
+                accessible-role: none;
             }
         }
     }
 
     i-touch-area := TouchArea {
         clicked => {
             if (root.checkable) {
```

### Comparing `slint-1.6.0a6/internal/compiler/widgets/fluent-base/checkbox.slint` & `slint-1.6.0a7/internal/compiler/widgets/fluent-base/checkbox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/fluent-base/combobox.slint` & `slint-1.6.0a7/internal/compiler/widgets/fluent-base/combobox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/fluent-base/components.slint` & `slint-1.6.0a7/internal/compiler/widgets/fluent-base/components.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/fluent-base/groupbox.slint` & `slint-1.6.0a7/internal/compiler/widgets/fluent-base/groupbox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/fluent-base/layouts.slint` & `slint-1.6.0a7/internal/compiler/widgets/fluent-base/layouts.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/fluent-base/lineedit.slint` & `slint-1.6.0a7/internal/compiler/widgets/fluent-base/lineedit.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/fluent-base/progressindicator.slint` & `slint-1.6.0a7/internal/compiler/widgets/fluent-base/progressindicator.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/fluent-base/scrollview.slint` & `slint-1.6.0a7/internal/compiler/widgets/fluent-base/scrollview.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/fluent-base/slider.slint` & `slint-1.6.0a7/internal/compiler/widgets/fluent-base/slider.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/fluent-base/spinbox.slint` & `slint-1.6.0a7/internal/compiler/widgets/fluent-base/spinbox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/fluent-base/spinner.slint` & `slint-1.6.0a7/internal/compiler/widgets/fluent-base/spinner.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/fluent-base/std-widgets-base.slint` & `slint-1.6.0a7/internal/compiler/widgets/fluent-base/std-widgets-base.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/fluent-base/std-widgets-impl.slint` & `slint-1.6.0a7/internal/compiler/widgets/fluent-base/std-widgets-impl.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/fluent-base/styling.slint` & `slint-1.6.0a7/internal/compiler/widgets/fluent-base/styling.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/fluent-base/switch.slint` & `slint-1.6.0a7/internal/compiler/widgets/fluent-base/switch.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/fluent-base/tableview.slint` & `slint-1.6.0a7/internal/compiler/widgets/fluent-base/tableview.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/fluent-base/tabwidget.slint` & `slint-1.6.0a7/internal/compiler/widgets/fluent-base/tabwidget.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/fluent-base/textedit.slint` & `slint-1.6.0a7/internal/compiler/widgets/fluent-base/textedit.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/material-base/button.slint` & `slint-1.6.0a7/internal/compiler/widgets/material-base/button.slint`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     min-width: max(40px, i-layout.min-width);
     forward-focus: i-state-layer;
 
     accessible-role: button;
     accessible-checkable: root.checkable;
     accessible-checked: root.checked;
     accessible-label: root.text;
-    accessible-action-default => { clicked(); }
+    accessible-action-default => { i-state-layer.clicked(); }
 
     states [
         disabled when !root.enabled : {
             i-background.background: MaterialPalette.foreground-alt;
             i-background.opacity: 0.12;
             root.text-opacity: 0.38;
             root.text-color: MaterialPalette.control-foreground;
@@ -84,12 +84,13 @@
         if (root.text != "") : Text {
             text: root.text;
             color: root.text-color;
             opacity: root.text-opacity;
             vertical-alignment: center;
             horizontal-alignment: center;
             font-weight: MaterialFontSettings.label-large.font-weight;
+            accessible-role: none;
 
             animate color { duration: 250ms; easing: ease; }
         }
     }
 }
```

### Comparing `slint-1.6.0a6/internal/compiler/widgets/material-base/checkbox.slint` & `slint-1.6.0a7/internal/compiler/widgets/material-base/checkbox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/material-base/combobox.slint` & `slint-1.6.0a7/internal/compiler/widgets/material-base/combobox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/material-base/components.slint` & `slint-1.6.0a7/internal/compiler/widgets/material-base/components.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/material-base/groupbox.slint` & `slint-1.6.0a7/internal/compiler/widgets/material-base/groupbox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/material-base/layouts.slint` & `slint-1.6.0a7/internal/compiler/widgets/material-base/layouts.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/material-base/lineedit.slint` & `slint-1.6.0a7/internal/compiler/widgets/material-base/lineedit.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/material-base/progressindicator.slint` & `slint-1.6.0a7/internal/compiler/widgets/material-base/progressindicator.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/material-base/scrollview.slint` & `slint-1.6.0a7/internal/compiler/widgets/material-base/scrollview.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/material-base/slider.slint` & `slint-1.6.0a7/internal/compiler/widgets/material-base/slider.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/material-base/spinbox.slint` & `slint-1.6.0a7/internal/compiler/widgets/material-base/spinbox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/material-base/spinner.slint` & `slint-1.6.0a7/internal/compiler/widgets/material-base/spinner.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/material-base/std-widgets-base.slint` & `slint-1.6.0a7/internal/compiler/widgets/material-base/std-widgets-base.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/material-base/std-widgets-impl.slint` & `slint-1.6.0a7/internal/compiler/widgets/material-base/std-widgets-impl.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/material-base/styling.slint` & `slint-1.6.0a7/internal/compiler/widgets/material-base/styling.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/material-base/switch.slint` & `slint-1.6.0a7/internal/compiler/widgets/material-base/switch.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/material-base/tableview.slint` & `slint-1.6.0a7/internal/compiler/widgets/material-base/tableview.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/material-base/tabwidget.slint` & `slint-1.6.0a7/internal/compiler/widgets/material-base/tabwidget.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/qt/button.slint` & `slint-1.6.0a7/internal/compiler/widgets/qt/button.slint`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,20 @@
 
     callback clicked <=> native.clicked;
 
     accessible-role: button;
     accessible-checkable: root.checkable;
     accessible-checked: root.checked;
     accessible-label: root.text;
-    accessible-action-default => { clicked(); }
+    accessible-action-default => {
+        if (root.checkable) {
+            root.checked = !root.checked;
+        }
+        clicked();
+    }
 
     forward-focus: native;
 
     HorizontalLayout {
         native := NativeButton {
             checkable: false;
             enabled: true;
```

### Comparing `slint-1.6.0a6/internal/compiler/widgets/qt/combobox.slint` & `slint-1.6.0a7/internal/compiler/widgets/qt/combobox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/qt/groupbox.slint` & `slint-1.6.0a7/internal/compiler/widgets/qt/groupbox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/qt/internal-scrollview.slint` & `slint-1.6.0a7/internal/compiler/widgets/qt/internal-scrollview.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/qt/layouts.slint` & `slint-1.6.0a7/internal/compiler/widgets/qt/layouts.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/qt/lineedit.slint` & `slint-1.6.0a7/internal/compiler/widgets/qt/lineedit.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/qt/scrollview.slint` & `slint-1.6.0a7/internal/compiler/widgets/qt/scrollview.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/qt/spinbox.slint` & `slint-1.6.0a7/internal/compiler/widgets/qt/spinbox.slint`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 // Copyright © SixtyFPS GmbH <info@slint.dev>
 // SPDX-License-Identifier: GPL-3.0-only OR LicenseRef-Slint-Royalty-free-1.2 OR LicenseRef-Slint-commercial
 
 export component SpinBox inherits NativeSpinBox {
+    value: root.minimum;
     accessible-role: spinbox;
     accessible-value: root.value;
     accessible-value-minimum: root.minimum;
     accessible-value-maximum: root.maximum;
     accessible-value-step: (root.maximum - root.minimum) / 100;
 
     accessible-action-set-value(v) => { if v.is-float() {update-value(v.to-float());} }
```

### Comparing `slint-1.6.0a6/internal/compiler/widgets/qt/spinner.slint` & `slint-1.6.0a7/internal/compiler/widgets/qt/spinner.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/qt/std-widgets.slint` & `slint-1.6.0a7/internal/compiler/widgets/qt/std-widgets.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/qt/tableview.slint` & `slint-1.6.0a7/internal/compiler/widgets/qt/tableview.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/widgets/qt/tabwidget.slint` & `slint-1.6.0a7/internal/compiler/widgets/qt/tabwidget.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/renderers/skia/Cargo.toml` & `slint-1.6.0a7/internal/renderers/skia/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/renderers/skia/LICENSES/GPL-3.0-only.txt` & `slint-1.6.0a7/internal/common/LICENSES/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/renderers/skia/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md` & `slint-1.6.0a7/internal/common/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/renderers/skia/LICENSES/LicenseRef-Slint-commercial.md` & `slint-1.6.0a7/internal/common/LICENSES/LicenseRef-Slint-commercial.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/renderers/skia/build.rs` & `slint-1.6.0a7/internal/renderers/skia/build.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/renderers/skia/cached_image.rs` & `slint-1.6.0a7/internal/renderers/skia/cached_image.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/renderers/skia/d3d_surface.rs` & `slint-1.6.0a7/internal/renderers/skia/d3d_surface.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/renderers/skia/itemrenderer.rs` & `slint-1.6.0a7/internal/renderers/skia/itemrenderer.rs`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 use std::pin::Pin;
 
 use super::{PhysicalBorderRadius, PhysicalLength, PhysicalPoint, PhysicalRect, PhysicalSize};
 use i_slint_core::graphics::boxshadowcache::BoxShadowCache;
 use i_slint_core::graphics::euclid::num::Zero;
 use i_slint_core::graphics::euclid::{self, Vector2D};
 use i_slint_core::item_rendering::{CachedRenderingData, ItemCache, ItemRenderer, RenderImage};
-use i_slint_core::items::{ImageFit, ImageRendering, ItemRc, Layer, Opacity, RenderingResult};
+use i_slint_core::items::{
+    ImageFit, ImageRendering, ItemRc, Layer, Opacity, RenderingResult, TextStrokeStyle,
+};
 use i_slint_core::lengths::{
     LogicalBorderRadius, LogicalLength, LogicalPoint, LogicalPx, LogicalRect, LogicalSize,
     LogicalVector, PhysicalPx, RectLengths, ScaleFactor, SizeLengths,
 };
 use i_slint_core::window::WindowInner;
 use i_slint_core::{Brush, Color};
 use skia_safe::{Matrix, TileMode};
@@ -452,29 +454,84 @@
             Some(paint) => paint,
             None => return,
         };
 
         let mut text_style = skia_safe::textlayout::TextStyle::new();
         text_style.set_foreground_paint(&paint);
 
+        let stroke_style = text.stroke_style();
+        let stroke_width = if text.stroke_width().get() != 0.0 {
+            (text.stroke_width() * self.scale_factor).get()
+        } else {
+            // Hairline stroke
+            1.0
+        };
+        let stroke_width = match stroke_style {
+            TextStrokeStyle::Outside => stroke_width * 2.0,
+            TextStrokeStyle::Center => stroke_width,
+        };
+
+        let mut text_stroke_style = skia_safe::textlayout::TextStyle::new();
+        let stroke_layout = match self.brush_to_paint(text.stroke(), max_width, max_height) {
+            Some(mut stroke_paint) => {
+                if text.stroke().is_transparent() {
+                    None
+                } else {
+                    stroke_paint.set_style(skia_safe::PaintStyle::Stroke);
+                    stroke_paint.set_stroke_width(stroke_width);
+                    // Set stroke cap/join/miter to match FemtoVG
+                    stroke_paint.set_stroke_cap(skia_safe::PaintCap::Butt);
+                    stroke_paint.set_stroke_join(skia_safe::PaintJoin::Miter);
+                    stroke_paint.set_stroke_miter(10.0);
+                    text_stroke_style.set_foreground_paint(&stroke_paint);
+                    Some(super::textlayout::create_layout(
+                        font_request.clone(),
+                        self.scale_factor,
+                        string,
+                        Some(text_stroke_style),
+                        Some(max_width),
+                        max_height,
+                        text.horizontal_alignment(),
+                        text.vertical_alignment(),
+                        text.wrap(),
+                        text.overflow(),
+                        None,
+                    ))
+                }
+            }
+            None => None,
+        };
+
         let (layout, layout_top_left) = super::textlayout::create_layout(
             font_request,
             self.scale_factor,
             string,
             Some(text_style),
             Some(max_width),
             max_height,
             text.horizontal_alignment(),
             text.vertical_alignment(),
             text.wrap(),
             text.overflow(),
             None,
         );
 
-        layout.paint(&mut self.canvas, to_skia_point(layout_top_left));
+        match (stroke_style, stroke_layout) {
+            (TextStrokeStyle::Outside, Some((stroke_layout, stroke_layout_top_left))) => {
+                stroke_layout.paint(&mut self.canvas, to_skia_point(stroke_layout_top_left));
+                layout.paint(&mut self.canvas, to_skia_point(layout_top_left));
+            }
+            (TextStrokeStyle::Center, Some((stroke_layout, stroke_layout_top_left))) => {
+                layout.paint(&mut self.canvas, to_skia_point(layout_top_left));
+                stroke_layout.paint(&mut self.canvas, to_skia_point(stroke_layout_top_left));
+            }
+            _ => {
+                layout.paint(&mut self.canvas, to_skia_point(layout_top_left));
+            }
+        };
     }
 
     fn draw_text_input(
         &mut self,
         text_input: std::pin::Pin<&i_slint_core::items::TextInput>,
         _self_rc: &i_slint_core::items::ItemRc,
         size: LogicalSize,
```

### Comparing `slint-1.6.0a6/internal/renderers/skia/lib.rs` & `slint-1.6.0a7/internal/renderers/skia/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/renderers/skia/metal_surface.rs` & `slint-1.6.0a7/internal/renderers/skia/metal_surface.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/renderers/skia/opengl_surface.rs` & `slint-1.6.0a7/internal/renderers/skia/opengl_surface.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/renderers/skia/software_surface.rs` & `slint-1.6.0a7/internal/renderers/skia/software_surface.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/renderers/skia/textlayout.rs` & `slint-1.6.0a7/internal/renderers/skia/textlayout.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/renderers/skia/vulkan_surface.rs` & `slint-1.6.0a7/internal/renderers/skia/vulkan_surface.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/Cargo.toml` & `slint-1.6.0a7/api/rs/slint/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -189,15 +189,15 @@
 i-slint-renderer-femtovg = { workspace = true, optional = true }
 
 [target.'cfg(target_os = "android")'.dependencies]
 i-slint-backend-android-activity = { workspace = true, optional = true }
 
 [dev-dependencies]
 slint-build = { path = "../build" }
-i-slint-backend-testing = { path = "../../../internal/backends/testing" }
+i-slint-backend-testing = { path = "../../../internal/backends/testing", features = ["internal"] }
 serde_json = "1.0.96"
 serde = { version = "1.0.163", features = ["derive"] }
 
 [target.'cfg(target_os = "linux")'.dependencies]
 # this line is there to add the "enable" feature by default, but only on linux
 i-slint-backend-qt = { workspace = true, features = [ "enable" ], optional = true }
```

### Comparing `slint-1.6.0a6/api/rs/slint/LICENSES/GPL-3.0-only.txt` & `slint-1.6.0a7/internal/renderers/femtovg/LICENSES/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md` & `slint-1.6.0a7/internal/renderers/femtovg/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/LICENSES/LicenseRef-Slint-commercial.md` & `slint-1.6.0a7/internal/renderers/femtovg/LICENSES/LicenseRef-Slint-commercial.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/LICENSES/MIT.txt` & `slint-1.6.0a7/internal/compiler/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/README.md` & `slint-1.6.0a7/api/rs/slint/README.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/android.rs` & `slint-1.6.0a7/api/rs/slint/android.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/compile_fail_tests.rs` & `slint-1.6.0a7/api/rs/slint/compile_fail_tests.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/building.md` & `slint-1.6.0a7/api/rs/slint/docs/building.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/development.md` & `slint-1.6.0a7/api/rs/slint/docs/development.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/install_qt.md` & `slint-1.6.0a7/api/rs/slint/docs/install_qt.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/README.md` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/README.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/CMakeLists.txt` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/SUMMARY.md` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/SUMMARY.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/conclusion.md` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/conclusion.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/creating_the_tiles_from_cpp.md` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/creating_the_tiles_from_cpp.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/from_one_to_multiple_tiles.md` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/from_one_to_multiple_tiles.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/game_logic_in_cpp.md` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/game_logic_in_cpp.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/getting_started.md` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/getting_started.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/at-solid.svg` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/at-solid.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/at.png` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/at.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/balance-scale-solid.svg` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/balance-scale-solid.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/balance-scale.png` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/balance-scale.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/bicycle-solid.svg` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/bicycle-solid.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/bicycle.png` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/bicycle.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/bus-solid.svg` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/bus-solid.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/bus.png` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/bus.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/cloud.png` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/cloud.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/cogs-solid.svg` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/cogs-solid.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/cogs.png` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/cogs.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/motorcycle-solid.svg` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/motorcycle-solid.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/motorcycle.png` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/motorcycle.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/tile_logo.png` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/tile_logo.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/icons/video.png` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/video.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/ideas_for_the_reader.md` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/ideas_for_the_reader.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/introduction.md` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/introduction.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/main_game_logic.cpp` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/main_game_logic.cpp`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/main_tiles_from_cpp.cpp` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/main_tiles_from_cpp.cpp`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/memory_game_logic.slint` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/memory_game_logic.slint`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
         width: parent.width;
         height: parent.height;
     }
 
     // Left curtain
     Rectangle {
         background: #193076;
+        x: 0px;
         width: open_curtain ? 0px : (parent.width / 2);
         height: parent.height;
         animate width { duration: 250ms; easing: ease-in; }
     }
 
     // Right curtain
     Rectangle {
```

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/memory_tile.md` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/memory_tile.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/memory_tiles_from_cpp.slint` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/memory_tiles_from_cpp.slint`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,15 @@
         width: parent.width;
         height: parent.height;
     }
 
     // Left curtain
     Rectangle {
         background: #193076;
+        x: 0px;
         width: open_curtain ? 0px : (parent.width / 2);
         height: parent.height;
         animate width { duration: 250ms; easing: ease-in; }
     }
 
     // Right curtain
     Rectangle {
```

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/cpp/src/polishing_the_tile.md` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/polishing_the_tile.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/SUMMARY.md` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/SUMMARY.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/conclusion.md` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/conclusion.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/creating_the_tiles_from_js.md` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/creating_the_tiles_from_js.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/from_one_to_multiple_tiles.md` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/from_one_to_multiple_tiles.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/game_logic_in_js.md` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/game_logic_in_js.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/getting_started.md` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/getting_started.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/at-solid.svg` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/at-solid.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/at.png` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/at.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/balance-scale-solid.svg` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/balance-scale-solid.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/balance-scale.png` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/balance-scale.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/bicycle-solid.svg` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/bicycle-solid.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/bicycle.png` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/bicycle.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/bus-solid.svg` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/bus-solid.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/bus.png` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/bus.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/cloud.png` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/cloud.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/cogs-solid.svg` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/cogs-solid.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/cogs.png` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/cogs.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/motorcycle-solid.svg` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/motorcycle-solid.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/motorcycle.png` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/motorcycle.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/tile_logo.png` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/tile_logo.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/icons/video.png` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/video.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/ideas_for_the_reader.md` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/ideas_for_the_reader.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/introduction.md` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/introduction.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/main_game_logic.js` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/main_game_logic.js`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/main_tiles_from_js.js` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/main_tiles_from_js.js`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/memory_game_logic.slint` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/memory_game_logic.slint`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
         width: parent.width;
         height: parent.height;
     }
 
     // Left curtain
     Rectangle {
         background: #193076;
+        x: 0px;
         width: open_curtain ? 0px : (parent.width / 2);
         height: parent.height;
         animate width { duration: 250ms; easing: ease-in; }
     }
 
     // Right curtain
     Rectangle {
```

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/memory_tile.md` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/memory_tile.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/memory_tiles_from_cpp.slint` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/memory_tiles_from_cpp.slint`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,15 @@
         width: parent.width;
         height: parent.height;
     }
 
     // Left curtain
     Rectangle {
         background: #193076;
+        x: 0px;
         width: open_curtain ? 0px : (parent.width / 2);
         height: parent.height;
         animate width { duration: 250ms; easing: ease-in; }
     }
 
     // Right curtain
     Rectangle {
```

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/node/src/polishing_the_tile.md` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/polishing_the_tile.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/quickstart/theme/head.hbs` & `slint-1.6.0a7/api/rs/slint/docs/quickstart/theme/head.hbs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/conf.py` & `slint-1.6.0a7/api/rs/slint/docs/reference/conf.py`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/index.rst` & `slint-1.6.0a7/api/rs/slint/docs/reference/index.rst`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/advanced/backend_linuxkms.md` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/advanced/backend_linuxkms.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/advanced/backend_qt.md` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/advanced/backend_qt.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/advanced/backend_winit.md` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/advanced/backend_winit.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/advanced/backends_and_renderers.md` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/advanced/backends_and_renderers.md`

 * *Files 0% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 - Suitable for Microcontrollers.
 - Some features haven't been implemented yet:
   * No support for `Path`.
   * No image rotation or smooth scaling.
   * No support for `drop-shadow-*` properties.
   * No support for `border-radius` in combination with `clip: true`.
   * No circular gradients.
+  * No text stroking/outlining.
 - Text rendering currently limited to western scripts.
 - Available in the [Winit backend](backend_winit.md).
 - Public [Rust](slint-rust:platform/software_renderer/) and [C++](slint-cpp:api/classslint_1_1platform_1_1SoftwareRenderer) API.
 
 ### FemtoVG Renderer
 
  - Highly portable.
```

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/advanced/debugging_techniques.md` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/advanced/debugging_techniques.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/advanced/style.md` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/advanced/style.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/introduction/index.md` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/introduction/index.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/introduction/supported_platforms.md` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/introduction/supported_platforms.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/builtins/callbacks.md` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/builtins/callbacks.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/builtins/elements.md` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/builtins/elements.md`

 * *Files 2% similar despite different names*

```diff
@@ -58,25 +58,33 @@
     }
 }
 ```
 
 ### Accessibility
 
 Use the following `accessible-` properties to make your items interact well with software like screen readers, braille terminals and other software to make your application accessible.
+`accessible-role` must be set in order to be able to set any other accessible property or callback.
 
 -   **`accessible-role`** (_in_ _enum [`AccessibleRole`](enums.md#accessiblerole)_): The role of the element. This property is mandatory to be able to use any other accessible properties. It should be set to a constant value. (default value: `none` for most elements, but `text` for the Text element)
 -   **`accessible-checkable`** (_in_ _bool_): Whether the element is can be checked or not.
 -   **`accessible-checked`** (_in_ _bool_): Whether the element is checked or not. This maps to the "checked" state of checkboxes, radio buttons, and other widgets.
 -   **`accessible-description`** (_in_ _string_): The description for the current element.
 -   **`accessible-label`** (_in_ _string_): The label for an interactive element. (default value: empty for most elements, or the value of the `text` property for Text elements)
 -   **`accessible-value-maximum`** (_in_ _float_): The maximum value of the item. This is used for example by spin boxes.
 -   **`accessible-value-minimum`** (_in_ _float_): The minimum value of the item.
 -   **`accessible-value-step`** (_in_ _float_) The smallest increment or decrement by which the current value can change. This corresponds to the step by which a handle on a slider can be dragged.
 -   **`accessible-value`** (_in_ _string_): The current value of the item.
 
+You can also use the following callbacks that are going to be called by the accessibility framework:
+
+-  **`accessible-action-default()`**: Invoked when the default action for this widget is requested (eg: pressed for a button).
+-  **`accessible-action-set-value(string)`**: Invoked when the user wants to change the accessible value.
+-  **`accessible-action-increment()`**: Invoked when the user requests to increment the value.
+-  **`accessible-action-decrement()`**: Invoked when the user requests to decrement the value.
+
 ### Drop Shadows
 
 To achieve the graphical effect of a visually elevated shape that shows a shadow effect underneath the frame of
 an element, it's possible to set the following `drop-shadow` properties:
 
 -   **`drop-shadow-blur`** (_in_ _length_): The radius of the shadow that also describes the level of blur applied to the shadow. Negative values are ignored and zero means no blur. (default value: 0)
 -   **`drop-shadow-color`** (_in_ _color_): The base color of the shadow to use. Typically that color is the starting color of a gradient that fades into transparency.
@@ -204,14 +212,15 @@
     behavior. Similarly, a disabled `FocusScope` does not accept the focus via tab focus traversal. A parent `FocusScope` will still receive key events from
     child `FocusScope`s that were rejected, even if `enabled` is set to false. (default value: true)
 
 ### Functions
 
 -   **`focus()`** Call this function to transfer keyboard focus to this `FocusScope`,
     to receive future [`KeyEvent`](structs.md#keyevent)s.
+-   **`clear-focus()`** Call this function to remove keyboard focus from this `FocusScope` if it currently has the focus. See also [](../concepts/focus.md).
 
 ### Callbacks
 
 -   **`key-pressed(KeyEvent) -> EventResult`**: Invoked when a key is pressed, the argument is a [`KeyEvent`](structs.md#keyevent) struct. The returned [`EventResult`](enums.md#eventresult) indicates whether to accept or ignore the event. Ignored events are
     forwarded to the parent element.
 -   **`key-released(KeyEvent) -> EventResult`**: Invoked when a key is released, the argument is a [`KeyEvent`](structs.md#keyevent) struct. The returned [`EventResult`](enums.md#eventresult) indicates whether to accept or ignore the event. Ignored events are
     forwarded to the parent element.
@@ -668,14 +677,15 @@
 -   **`text`** (_in-out_ _string_): The text rendered and editable by the user.
 -   **`vertical-alignment`** (_in_ _enum [`TextVerticalAlignment`](enums.md#textverticalalignment)_): The vertical alignment of the text.
 -   **`wrap`** (_in_ _enum [`TextWrap`](enums.md#textwrap)_): The way the text input wraps. Only makes sense when `single-line` is false. (default value: no-wrap)
 
 ### Functions
 
 -   **`focus()`** Call this function to focus the text input and make it receive future keyboard events.
+-   **`clear-focus()`** Call this function to remove keyboard focus from this `TextInput` if it currently has the focus. See also [](../concepts/focus.md).
 -   **`set-selection-offsets(int, int)`** Selects the text between two UTF-8 offsets.
 -   **`select-all()`** Selects all text.
 -   **`clear-selection()`** Clears the selection.
 -   **`copy()`** Copies the selected text to the clipboard.
 -   **`cut()`** Copies the selected text to the clipboard and removes it from the editable area.
 -   **`paste()`** Pastes the text content of the clipboard at the cursor position.
 
@@ -698,15 +708,16 @@
     }
 }
 ```
 
 ## `Text`
 
 The `Text` element is responsible for rendering text. Besides the `text` property, that specifies which text to render,
-it also allows configuring different visual aspects through the `font-family`, `font-size`, `font-weight` and `color` properties.
+it also allows configuring different visual aspects through the `font-family`, `font-size`, `font-weight`, `color`, and
+`stroke` properties.
 
 The `Text` element can break long text into multiple lines of text. A line feed character (`\n`) in the string of the `text`
 property will trigger a manual line break. For automatic line breaking you need to set the `wrap` property to a value other than
 `no-wrap`, and it's important to specify a `width` and `height` for the `Text` element, in order to know where to break. It's
 recommended to place the `Text` element in a layout and let it set the `width` and `height` based on the available screen space
 and the text itself.
 
@@ -719,14 +730,17 @@
 -   **`font-italic`** (_in_ _bool_): Whether or not the font face should be drawn italicized or not. (default value: false)
 -   **`horizontal-alignment`** (_in_ _enum [`TextHorizontalAlignment`](enums.md#texthorizontalalignment)_): The horizontal alignment of the text.
 -   **`letter-spacing`** (_in_ _length_): The letter spacing allows changing the spacing between the glyphs. A positive value increases the spacing and a negative value decreases the distance. (default value: 0)
 -   **`overflow`** (_in_ _enum [`TextOverflow`](enums.md#textoverflow)_): What happens when the text overflows (default value: clip).
 -   **`text`** (_in_ _[string](../syntax/types.md#strings)_): The text rendered.
 -   **`vertical-alignment`** (_in_ _enum [`TextVerticalAlignment`](enums.md#textverticalalignment)_): The vertical alignment of the text.
 -   **`wrap`** (_in_ _enum [`TextWrap`](enums.md#textwrap)_): The way the text wraps (default value: `no-wrap`).
+-   **`stroke`** (_in_ _brush_): The brush used for the text outline (default value: `transparent`).
+-   **`stroke-width`** (_in_ _length_): The width of the text outline. If the width is zero, then a hairline stroke (1 physical pixel) will be rendered.
+-   **`stroke-style`** (_in_ _enum [`TextStrokeStyle`](enums.md#textstrokestyle)_): The style/alignment of the text outline (default value: `outside`).
 
 ### Example
 
 This example shows the text "Hello World" in red, using the default font:
 
 ```slint
 export component Example inherits Window {
```

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/builtins/functions.md` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/builtins/functions.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/builtins/globals.md` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/builtins/globals.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/builtins/namespaces.md` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/builtins/namespaces.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/concepts/container.md` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/concepts/container.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/concepts/file.md` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/concepts/file.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/concepts/focus.md` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/concepts/focus.md`

 * *Files 9% similar despite different names*

```diff
@@ -20,14 +20,37 @@
         input := TextInput {
             text: "I am a text input field";
         }
     }
 }
 ```
 
+Similarly, you can manually clear the focus on an element that's currently focused, by calling `clear-focus()`:
+
+```slint
+import { Button } from "std-widgets.slint";
+
+export component App inherits Window {
+    VerticalLayout {
+        alignment: start;
+        Button {
+            text: "press me";
+            clicked => { input.clear-focus(); }
+        }
+        input := TextInput {
+            text: "I am a text input field";
+        }
+    }
+}
+```
+
+After the focus is cleared, keyboard input to the window is discarded, until another element is explicitly
+focused. For example by calling `focus()`, an element acquiring focus when the user clicks on it, or when
+pressing tab and the first focusable element is found.
+
 If you have wrapped the `TextInput` in a component, then you can forward such a focus activation
 using the `forward-focus` property to refer to the element that should receive it:
 
 ```slint
 import { Button } from "std-widgets.slint";
 
 component LabeledInput inherits GridLayout {
```

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/concepts/fonts.md` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/concepts/fonts.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/concepts/layouting.md` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/concepts/layouting.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/concepts/purity.md` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/concepts/purity.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/concepts/translations.md` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/concepts/translations.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/index.rst` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/index.rst`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/animations.md` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/animations.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/callbacks.md` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/callbacks.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/expressions.md` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/expressions.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/functions.md` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/functions.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/globals.md` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/globals.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/legacy_syntax.md` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/legacy_syntax.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/modules.md` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/modules.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/properties.md` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/properties.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/repetitions.md` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/repetitions.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/statements.md` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/statements.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/states.md` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/states.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/syntax/types.md` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/types.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/button.md` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/button.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/checkbox.md` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/checkbox.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/combobox.md` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/combobox.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/groupbox.md` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/groupbox.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/index.rst` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/index.rst`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/lineedit.md` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/lineedit.md`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 -   **`read-only`** (_in_ _bool_): When set to true, text editing via keyboard and mouse is disabled but
     selecting text is still enabled as well as editing text programatically (default value: `false`)
 -   **`text`** (_in-out_ _string_): The text being edited
 
 ### Functions
 
 -   **`focus()`** Call this function to focus the LineEdit and make it receive future keyboard events.
+-   **`clear-focus()`** Call this function to remove keyboard focus from this `LineEdit` if it currently has the focus. See also [](../concepts/focus.md).
 -   **`set-selection-offsets(int, int)`** Selects the text between two UTF-8 offsets.
 -   **`select-all()`** Selects all text.
 -   **`clear-selection()`** Clears the selection.
 -   **`copy()`** Copies the selected text to the clipboard.
 -   **`cut()`** Copies the selected text to the clipboard and removes it from the editable area.
 -   **`paste()`** Pastes the text content of the clipboard at the cursor position.
```

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/listview.md` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/listview.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/progressindicator.md` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/progressindicator.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/scrollview.md` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/scrollview.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/slider.md` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/slider.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <!-- Copyright © SixtyFPS GmbH <info@slint.dev> ; SPDX-License-Identifier: MIT -->
 ## `Slider`
 
 ### Properties
 
 -   **`enabled`**: (_in_ _bool_): Defaults to true. You can't interact with the slider if enabled is false.
 -   **`has-focus`**: (_out_ _bool_): Set to true when the slider currently has the focus
--   **`value`** (_in-out_ _float_): The value.
+-   **`value`** (_in-out_ _float_): The value. Defaults to the minimum.
 -   **`minimum`** (_in_ _float_): The minimum value (default: 0)
 -   **`maximum`** (_in_ _float_): The maximum value (default: 100)
 -   **`orientation`** (_in_ _enum [`Orientation`](../builtins/enums.md#orientation)_): If set to true the Slider is displayed vertical (default: horizontal).
 
 ### Callbacks
 
 -   **`changed(float)`**: The value was changed
```

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/spinbox.md` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/spinbox.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <!-- Copyright © SixtyFPS GmbH <info@slint.dev> ; SPDX-License-Identifier: MIT -->
 ## `SpinBox`
 
 ### Properties
 
 -   **`enabled`**: (_in_ _bool_): Defaults to true. You can't interact with the spinbox if enabled is false.
 -   **`has-focus`**: (_out_ _bool_): Set to true when the spinbox currently has the focus
--   **`value`** (_in-out_ _int_): The value.
+-   **`value`** (_in-out_ _int_): The value. Defaults to the minimum.
 -   **`minimum`** (_in_ _int_): The minimum value (default: 0).
 -   **`maximum`** (_in_ _int_): The maximum value (default: 100).
 
 ### Callbacks
 
 - **`edited(int)`**: Emitted when the value has changed because the user modified it
```

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/spinner.md` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/spinner.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/standardbutton.md` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/standardbutton.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/standardlistview.md` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/standardlistview.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/standardtableview.md` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/standardtableview.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/switch.md` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/switch.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/tabwidget.md` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/tabwidget.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/textedit.md` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/textedit.md`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 -   **`read-only`** (_in_ _bool_): When set to true, text editing via keyboard and mouse is disabled but selecting text is still enabled as well as editing text programmatically (default value: `false`)
 -   **`wrap`** (_in_ _enum [`TextWrap`](../builtins/enums.md#textwrap)_): The way the text wraps (default: word-wrap).
 -   **`horizontal-alignment`** (_in_ _enum [`TextHorizontalAlignment`](../builtins/enums.md#texthorizontalalignment)_): The horizontal alignment of the text.
 
 ### Functions
 
 -   **`focus()`** Call this function to focus the TextEdit and make it receive future keyboard events.
+-   **`clear-focus()`** Call this function to remove keyboard focus from this `TextEdit` if it currently has the focus. See also [](../concepts/focus.md).
 -   **`set-selection-offsets(int, int)`** Selects the text between two UTF-8 offsets.
 -   **`select-all()`** Selects all text.
 -   **`clear-selection()`** Clears the selection.
 -   **`copy()`** Copies the selected text to the clipboard.
 -   **`cut()`** Copies the selected text to the clipboard and removes it from the editable area.
 -   **`paste()`** Pastes the text content of the clipboard at the cursor position.
```

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/language/widgets/widgets.md` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/widgets.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/reference/src/recipes/recipes.md` & `slint-1.6.0a7/api/rs/slint/docs/reference/src/recipes/recipes.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/resources/slint-docs-highlight.html` & `slint-1.6.0a7/api/rs/slint/docs/resources/slint-docs-highlight.html`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/resources/slint-docs-preview.html` & `slint-1.6.0a7/api/rs/slint/docs/resources/slint-docs-preview.html`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/site/index.html` & `slint-1.6.0a7/api/rs/slint/docs/site/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -8,61 +8,67 @@
         <meta name="author" content="SixtyFPS GmbH" />
 
         <!--====== Favicon Icon ======-->
         <link rel="shortcut icon" href="https://slint.dev/assets/img/favicon.ico">
         <link rel="icon" type="image/x-icon" href="https://slint.dev/assets/img/favicon.svg">
 
         <!-- ===== All CSS files ===== -->
-        <link rel="stylesheet" href="https://slint.dev/assets/css/style.css?v=1.11.56" />
+        <link rel="stylesheet" href="https://slint.dev/assets/css/style.css?v=1.12.0" />
         
 
         <!-- ===== Header from individual pages ===== -->
         
         <title>Slint Developer Documentation</title>
         <meta name="description" content="The developer documentation page of Slint." />
     
     </head>
 
     <body>
         <script>
             /* Check if dark theme is selected */
             if (localStorage.getItem('theme') === 'dark') {
-              document.documentElement.classList.add('dark');
+                document.documentElement.classList.add('dark');
             }
             else if (localStorage.getItem('theme') === 'light') {
-              document.documentElement.classList.add('light');
+                document.documentElement.classList.add('light');
             }
-          </script>
+        </script>
 
         <div class="wrap">
             <!-- ====== Header Start ====== -->
             <header class="top">
                 <div class="header-wrap">
 
                     <a href="https://slint.dev/index.html" class="logo">Slint</a>
 
                     <nav class="main-navi">
 
                         <ul>
-                            <li id="use-cases"><a href="https://slint.dev/use-cases.html">Use Cases</a></li>
+                            <li class="navi-item-has-children" id="use-cases"><a href="#">Use Cases</a>
+                                <ul>
+                                    <li id="demos"><a href="https://slint.dev/demos.html">Demos</a></li>
+                                    <li id="supported-boards"><a href="https://slint.dev/supported-boards.html">Embedded</a></li>
+                                    <li id="use-cases"><a href="https://slint.dev/use-cases.html">Cross Platform</a></li>
+                                </ul>
+                            </li>
                             <li id="pricing"><a href="https://slint.dev/pricing.html">Pricing</a></li>
                             <li id="blog"><a href="https://slint.dev/blog">Blog</a></li>
                             <li id="docs"><a href="https://slint.dev/docs.html">Docs</a></li>
                             <li class="navi-item-has-children" id="resources"><a href="#">Resources</a>
                                 <ul>
-                                    <li id="demos"><a href="https://slint.dev/demos.html">Demos</a></li>
-                                    <li id="partners"><a href="https://slint.dev/partners.html">Partners</a></li>
-                                    <li id="community"><a href="https://slint.dev/community.html">Community</a></li>
                                     <li id="success"><a href="https://slint.dev/success">Success Stories</a></li>
-                                    <li id="supported-boards"><a href="https://slint.dev/supported-boards.html">Supported Boards</a></li>
-                                  </ul>
+                                    <li id="community"><a href="https://slint.dev/community.html">Community</a></li>
+                                    <li id="partners"><a href="https://slint.dev/partners.html">Partners</a></li>
+                                    <li id="events"><a href="https://slint.dev/events.html">Events</a></li>    
+                                </ul>
                             </li>
                             <!-- <li class="search"><a href="https://slint.dev/search-results.html">Search</a></li> -->
                             <li class="theme theme-light"><a href="#">Theme</a></li>
-                            <li class="btn"><a href="https://slint.dev/get-started.html">Get Started</a></li>
+                            <li class="btn btn-blue"><a href="https://slint.dev/get-started.html">Get Started</a></li>
+                            <li class="btn btn-white"><a href="https://slint.dev/contact.html">Contact Us</a></li>
                         </ul>
 
                     </nav>
 
                     <!-- <a href="https://slint.dev/search-results.html" class="search-mobile">Search</a> -->
 
                     <button class="hamburger" aria-label="menu" aria-expanded="false" aria-controls="nav">
@@ -97,23 +103,23 @@
                 <div class="col-wrap">
                     <div class="col-1">
                         <h2>Browse</h2>
                         <p>Whether you’re developing the UI or the backend, our documentation will guide you.</p>
                     </div>
                 </div>
                 <div class="col-wrap">
-                    <div class="col-2">
+                    <div id="slint-lang" class="col-2">
                         <div class="price-box">
                             <h5>DSL</h5>
                             <h4>Slint</h4>
                             <p><img src="https://slint.dev/assets/img/slint-favicon.svg"></p>
                             <p><a href="slint" class="btn doc">Language</a></p>
                         </div><!-- .price-box -->
                     </div><!-- .col-2 -->
-                    <div class="col-2">
+                    <div id="prog-lang" class="col-2">
                         <div class="col-wrap">
                             <div class="price-box">
                                 <h5>APIs</h5>
                                 <h4>Using Rust</h4>
                                 <p><img src="https://slint.dev/assets/img/rust-logo.svg"></p>
                                 <p><a href="rust/slint" class="btn doc">API</a></p>
                                 <p><a href="quickstart/rust" class="btn doc">QuickStart</a></p>
@@ -137,16 +143,17 @@
                                 <p><a href="https://github.com/slint-ui/slint-nodejs-template" class="btn" target="_blank">Project Template</a></p>
                             </div><!-- .price-box -->
                         </div><!-- .col-wrap -->
                     </div><!-- .col-2 -->
                 </div><!-- .col-wrap -->
             </section>
 
-            <section class="one-column" style="padding: 50px 0 2em;">
-                <p class="cta"><a href="https://slint.dev/contact.html" class="btn blue btn-center">Contact Us</a></p>
+            <section class="one-column mobile-only" style="padding: 50px 0 2em;">
+                <p class="cta"><a href="https://slint.dev/get-started.html" class="btn blue btn-center">Get Started</a></p>
+                <p class="cta"><a href="https://slint.dev/contact.html" class="btn btn-center">Contact Us</a></p>
             </section>
 
         </main>
     
 
             <!-- ====== Footer Start ====== -->
             <footer>
@@ -226,8 +233,8 @@
         </div><!-- .wrap -->
 
         <!-- ====== All Javascript Files ====== -->
         <script src="https://slint.dev/assets/js/script.js?ver=1.2.20"></script>
         
     </body>
 
-</html>
+</html>
```

#### html2text {}

```diff
@@ -1,20 +1,23 @@
 _S_l_i_n_t
     * _U_s_e_ _C_a_s_e_s
+          o _D_e_m_o_s
+          o _E_m_b_e_d_d_e_d
+          o _C_r_o_s_s_ _P_l_a_t_f_o_r_m
     * _P_r_i_c_i_n_g
     * _B_l_o_g
     * _D_o_c_s
     * _R_e_s_o_u_r_c_e_s
-          o _D_e_m_o_s
-          o _P_a_r_t_n_e_r_s
-          o _C_o_m_m_u_n_i_t_y
           o _S_u_c_c_e_s_s_ _S_t_o_r_i_e_s
-          o _S_u_p_p_o_r_t_e_d_ _B_o_a_r_d_s
+          o _C_o_m_m_u_n_i_t_y
+          o _P_a_r_t_n_e_r_s
+          o _E_v_e_n_t_s
     * _T_h_e_m_e
     * _G_e_t_ _S_t_a_r_t_e_d
+    * _C_o_n_t_a_c_t_ _U_s
 ************ DDooccuummeennttaattiioonn ************
 Version: VERSIONVisit _S_l_i_n_t_ _D_o_c_u_m_e_n_t_a_t_i_o_n for other versions.
 ********** BBrroowwssee **********
 Whether you’re developing the UI or the backend, our documentation will guide
 you.
 **** DDSSLL ****
 ****** SSlliinntt ******
@@ -35,14 +38,15 @@
 _P_r_o_j_e_c_t_ _T_e_m_p_l_a_t_e
 **** AAPPIIss ****
 ****** UUssiinngg NNooddeeJJSS ((bbeettaa)) ******
 [https://slint.dev/assets/img/nodejs_logo.svg]
 _A_P_I
 _Q_u_i_c_k_S_t_a_r_t
 _P_r_o_j_e_c_t_ _T_e_m_p_l_a_t_e
+_G_e_t_ _S_t_a_r_t_e_d
 _C_o_n_t_a_c_t_ _U_s
 _[_S_l_i_n_t_]
 _[_T_w_i_t_t_e_r_]_[_L_i_n_k_e_d_i_n_]_[_M_a_s_t_o_d_o_n_]
 [Annual Ross index]
   About
       _U_s
       _E_v_e_n_t_s
```

### Comparing `slint-1.6.0a6/api/rs/slint/docs/testing.md` & `slint-1.6.0a7/api/rs/slint/docs/testing.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/torizon.md` & `slint-1.6.0a7/api/rs/slint/docs/torizon.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs/triage.md` & `slint-1.6.0a7/api/rs/slint/docs/triage.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/docs.rs` & `slint-1.6.0a7/api/rs/slint/docs.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/lib.rs` & `slint-1.6.0a7/api/rs/slint/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/mcu.md` & `slint-1.6.0a7/api/rs/slint/mcu.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/slint/private_unstable_api.rs` & `slint-1.6.0a7/api/rs/slint/private_unstable_api.rs`

 * *Files 1% similar despite different names*

```diff
@@ -199,15 +199,17 @@
     };
     pub use i_slint_core::items::*;
     pub use i_slint_core::layout::*;
     pub use i_slint_core::lengths::{
         logical_position_to_api, LogicalLength, LogicalPoint, LogicalRect,
     };
     pub use i_slint_core::model::*;
-    pub use i_slint_core::properties::{set_state_binding, Property, PropertyTracker, StateInfo};
+    pub use i_slint_core::properties::{
+        set_state_binding, ChangeTracker, Property, PropertyTracker, StateInfo,
+    };
     pub use i_slint_core::slice::Slice;
     pub use i_slint_core::window::{
         InputMethodRequest, WindowAdapter, WindowAdapterRc, WindowInner,
     };
     pub use i_slint_core::Color;
     pub use i_slint_core::Coord;
     pub use i_slint_core::ItemTreeVTable_static;
```

### Comparing `slint-1.6.0a6/api/rs/slint/tests/partial_renderer.rs` & `slint-1.6.0a7/api/rs/slint/tests/partial_renderer.rs`

 * *Files 5% similar despite different names*

```diff
@@ -37,23 +37,26 @@
 #[track_caller]
 fn do_test_render_region(renderer: &SoftwareRenderer, x: i32, y: i32, x2: i32, y2: i32) {
     let mut buffer = vec![TestPixel(false); 500 * 500];
     let r = renderer.render(buffer.as_mut_slice(), 500);
     assert_eq!(r.bounding_box_size(), PhysicalSize { width: (x2 - x) as _, height: (y2 - y) as _ });
     assert_eq!(r.bounding_box_origin(), PhysicalPosition { x, y });
 
+    let mut has_one_pixel = false;
     for py in 0..500 {
         for px in 0..500 {
-            assert_eq!(
-                buffer[py * 500 + px].0,
-                (x..x2).contains(&(px as i32)) && (y..y2).contains(&(py as i32)),
-                "unexpected value at {px},{py}"
-            )
+            let in_bounding_box = (x..x2).contains(&(px as i32)) && (y..y2).contains(&(py as i32));
+            if !in_bounding_box {
+                assert!(!buffer[py * 500 + px].0, "Something written outside of bounding box in  {px},{py}   - (x={x},y={y},x2={x2},y2={y2})")
+            } else if buffer[py * 500 + px].0 {
+                has_one_pixel = true;
+            }
         }
     }
+    assert!(has_one_pixel, "Nothing was rendered");
 }
 
 #[test]
 fn simple() {
     slint::slint! {
         export component Ui inherits Window {
             in property <color> c: yellow;
```

### Comparing `slint-1.6.0a6/api/rs/slint/tests/show_strongref.rs` & `slint-1.6.0a7/api/rs/slint/tests/show_strongref.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 // Copyright © SixtyFPS GmbH <info@slint.dev>
 // SPDX-License-Identifier: GPL-3.0-only OR LicenseRef-Slint-Royalty-free-1.2 OR LicenseRef-Slint-commercial
 
 use ::slint::slint;
 
 #[test]
 fn show_maintains_strong_reference() {
-    i_slint_backend_testing::init_with_event_loop();
+    i_slint_backend_testing::init_integration_test();
 
     slint!(export component TestWindow inherits Window {
         callback root-clicked();
         TouchArea {
             clicked => { root.root-clicked(); }
         }
     });
```

### Comparing `slint-1.6.0a6/api/rs/slint/tests/simple_macro.rs` & `slint-1.6.0a7/api/rs/slint/tests/simple_macro.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 // Copyright © SixtyFPS GmbH <info@slint.dev>
 // SPDX-License-Identifier: GPL-3.0-only OR LicenseRef-Slint-Royalty-free-1.2 OR LicenseRef-Slint-commercial
 
 use ::slint::slint;
 
 #[test]
 fn simple_window() {
-    i_slint_backend_testing::init();
+    i_slint_backend_testing::init_no_event_loop();
     slint!(export component X inherits Window{});
     X::new().unwrap();
 }
 #[test]
 fn empty_stuff() {
     slint!();
     slint!(export struct Hei { abcd: bool });
     slint!(export global G { });
 }
 
 #[test]
 fn test_serialize_deserialize_struct() {
-    i_slint_backend_testing::init();
+    i_slint_backend_testing::init_no_event_loop();
     slint! {
 
         @rust-attr(derive(serde::Serialize, serde::Deserialize))
         export enum TestEnum {
             hello, world, xxx
         }
```

### Comparing `slint-1.6.0a6/api/rs/slint/tests/spawn_local.rs` & `slint-1.6.0a7/api/rs/slint/tests/spawn_local.rs`

 * *Files 5% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             }
         }
     }
 }
 
 #[test]
 fn main() {
-    i_slint_backend_testing::init_with_event_loop();
+    i_slint_backend_testing::init_integration_test();
 
     slint::invoke_from_event_loop(|| {
         let handle = slint::spawn_local(async { String::from("Hello") }).unwrap();
         slint::spawn_local(async move { panic!("Aborted task") }).unwrap().abort();
         let handle2 = slint::spawn_local(async move { handle.await + ", World" }).unwrap();
         std::thread::spawn(move || {
             let x = executor::block_on(handle2);
```

### Comparing `slint-1.6.0a6/api/rs/slint/type-mappings.md` & `slint-1.6.0a7/api/rs/slint/type-mappings.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/helper_crates/const-field-offset/macro/Cargo.toml` & `slint-1.6.0a7/helper_crates/const-field-offset/macro/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/helper_crates/const-field-offset/macro/macro.rs` & `slint-1.6.0a7/helper_crates/const-field-offset/macro/macro.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/macros/Cargo.toml` & `slint-1.6.0a7/api/rs/macros/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/macros/LICENSES/GPL-3.0-only.txt` & `slint-1.6.0a7/internal/backends/selector/LICENSES/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/macros/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md` & `slint-1.6.0a7/internal/backends/selector/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/macros/LICENSES/LicenseRef-Slint-commercial.md` & `slint-1.6.0a7/internal/backends/selector/LICENSES/LicenseRef-Slint-commercial.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/macros/lib.rs` & `slint-1.6.0a7/api/rs/macros/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/parser-test-macro/README.md` & `slint-1.6.0a7/internal/compiler/parser-test-macro/README.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/compiler/parser-test-macro/lib.rs` & `slint-1.6.0a7/internal/compiler/parser-test-macro/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/common/Cargo.toml` & `slint-1.6.0a7/internal/common/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/common/LICENSES/GPL-3.0-only.txt` & `slint-1.6.0a7/internal/core/LICENSES/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/common/LICENSES/LicenseRef-DejaVu-Font.txt` & `slint-1.6.0a7/internal/common/LICENSES/LicenseRef-DejaVu-Font.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/common/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md` & `slint-1.6.0a7/internal/core/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/common/LICENSES/LicenseRef-Slint-commercial.md` & `slint-1.6.0a7/internal/core/LICENSES/LicenseRef-Slint-commercial.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/common/README.md` & `slint-1.6.0a7/internal/common/README.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/common/builtin_structs.rs` & `slint-1.6.0a7/internal/common/builtin_structs.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/common/enums.rs` & `slint-1.6.0a7/internal/common/enums.rs`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,22 @@
             enum TextOverflow {
                 /// The text will simply be clipped.
                 Clip,
                 /// The text will be elided with `…`.
                 Elide,
             }
 
+            /// This enum describes the positioning of a text stroke relative to the border of the glyphs in a [`Text`](elements.md#text).
+            enum TextStrokeStyle {
+                /// The inside edge of the stroke is at the outer edge of the text.
+                Outside,
+                /// The center line of the stroke is at the outer edge of the text, like in Adobe Illustrator.
+                Center,
+            }
+
             /// This enum describes whether an event was rejected or accepted by an event handler.
             enum EventResult {
                 /// The event is rejected by this event handler and may then be handled by the parent item
                 Reject,
                 /// The event is accepted and won't be processed further
                 Accept,
             }
```

### Comparing `slint-1.6.0a6/internal/common/key_codes.rs` & `slint-1.6.0a7/internal/common/key_codes.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/common/lib.rs` & `slint-1.6.0a7/internal/common/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/common/sharedfontdb/DejaVuSans.ttf` & `slint-1.6.0a7/internal/common/sharedfontdb/DejaVuSans.ttf`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/common/sharedfontdb/fontconfig.rs` & `slint-1.6.0a7/internal/common/sharedfontdb/fontconfig.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/common/sharedfontdb.rs` & `slint-1.6.0a7/internal/common/sharedfontdb.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/android-activity/Cargo.toml` & `slint-1.6.0a7/internal/backends/android-activity/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/android-activity/LICENSES/GPL-3.0-only.txt` & `slint-1.6.0a7/internal/backends/winit/LICENSES/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/android-activity/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md` & `slint-1.6.0a7/internal/backends/winit/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/android-activity/LICENSES/LicenseRef-Slint-commercial.md` & `slint-1.6.0a7/internal/backends/winit/LICENSES/LicenseRef-Slint-commercial.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/android-activity/README.md` & `slint-1.6.0a7/internal/backends/android-activity/README.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/android-activity/androidwindowadapter.rs` & `slint-1.6.0a7/internal/backends/android-activity/androidwindowadapter.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/android-activity/build.rs` & `slint-1.6.0a7/internal/backends/android-activity/build.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/android-activity/java/SlintAndroidJavaHelper.java` & `slint-1.6.0a7/internal/backends/android-activity/java/SlintAndroidJavaHelper.java`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/android-activity/javahelper.rs` & `slint-1.6.0a7/internal/backends/android-activity/javahelper.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/android-activity/lib.rs` & `slint-1.6.0a7/internal/backends/android-activity/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/linuxkms/Cargo.toml` & `slint-1.6.0a7/internal/backends/linuxkms/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/linuxkms/LICENSES/GPL-3.0-only.txt` & `slint-1.6.0a7/internal/renderers/skia/LICENSES/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/linuxkms/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md` & `slint-1.6.0a7/internal/renderers/skia/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/linuxkms/LICENSES/LicenseRef-Slint-commercial.md` & `slint-1.6.0a7/internal/renderers/skia/LICENSES/LicenseRef-Slint-commercial.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/linuxkms/LICENSES/MIT.txt` & `slint-1.6.0a7/helper_crates/const-field-offset/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/linuxkms/calloop_backend/input.rs` & `slint-1.6.0a7/internal/backends/linuxkms/calloop_backend/input.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/linuxkms/calloop_backend.rs` & `slint-1.6.0a7/internal/backends/linuxkms/calloop_backend.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 // Copyright © SixtyFPS GmbH <info@slint.dev>
 // SPDX-License-Identifier: GPL-3.0-only OR LicenseRef-Slint-Royalty-free-1.2 OR LicenseRef-Slint-commercial
 
 use std::cell::RefCell;
 #[cfg(not(feature = "libseat"))]
 use std::fs::OpenOptions;
-use std::os::fd::{AsFd, BorrowedFd, OwnedFd, RawFd};
+use std::os::fd::OwnedFd;
 #[cfg(feature = "libseat")]
-use std::os::fd::{AsRawFd, FromRawFd};
+use std::os::fd::{AsFd, AsRawFd, FromRawFd};
 #[cfg(not(feature = "libseat"))]
 use std::os::unix::fs::OpenOptionsExt;
 use std::rc::Rc;
 use std::sync::atomic::AtomicBool;
 use std::sync::{Arc, Mutex};
 
 use calloop::EventLoop;
@@ -297,19 +297,8 @@
         }
     }
 }
 
 #[derive(Default)]
 pub struct LoopData {}
 
-struct Device {
-    // in the future, use this from libseat: device_id: i32,
-    fd: RawFd,
-}
-
-impl AsFd for Device {
-    fn as_fd(&self) -> std::os::fd::BorrowedFd<'_> {
-        unsafe { BorrowedFd::borrow_raw(self.fd) }
-    }
-}
-
 pub type EventLoopHandle<'a> = calloop::LoopHandle<'a, LoopData>;
```

### Comparing `slint-1.6.0a6/internal/backends/linuxkms/display/gbmdisplay.rs` & `slint-1.6.0a7/internal/backends/linuxkms/display/gbmdisplay.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/linuxkms/display/swdisplay.rs` & `slint-1.6.0a7/internal/backends/linuxkms/display/swdisplay.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/linuxkms/display/vulkandisplay.rs` & `slint-1.6.0a7/internal/backends/linuxkms/display/vulkandisplay.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/linuxkms/display.rs` & `slint-1.6.0a7/internal/backends/linuxkms/display.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/linuxkms/drmoutput.rs` & `slint-1.6.0a7/internal/backends/linuxkms/drmoutput.rs`

 * *Files 7% similar despite different names*

```diff
@@ -19,25 +19,14 @@
     }
 }
 
 impl drm::Device for SharedFd {}
 
 impl drm::control::Device for SharedFd {}
 
-struct OwnedFramebufferHandle {
-    handle: drm::control::framebuffer::Handle,
-    device: SharedFd,
-}
-
-impl Drop for OwnedFramebufferHandle {
-    fn drop(&mut self) {
-        self.device.destroy_framebuffer(self.handle).ok();
-    }
-}
-
 #[derive(Default)]
 enum PageFlipState {
     #[default]
     NoFrameBufferPosted,
     InitialBufferPosted,
     WaitingForPageFlip {
         _buffer_to_keep_alive_until_flip: Box<dyn Buffer>,
```

### Comparing `slint-1.6.0a6/internal/backends/linuxkms/fullscreenwindowadapter.rs` & `slint-1.6.0a7/internal/backends/linuxkms/fullscreenwindowadapter.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/linuxkms/lib.rs` & `slint-1.6.0a7/internal/backends/linuxkms/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/linuxkms/noop_backend.rs` & `slint-1.6.0a7/internal/backends/linuxkms/noop_backend.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/linuxkms/renderer/femtovg.rs` & `slint-1.6.0a7/internal/backends/linuxkms/renderer/femtovg.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/linuxkms/renderer/skia.rs` & `slint-1.6.0a7/internal/backends/linuxkms/renderer/skia.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core-macros/Cargo.toml` & `slint-1.6.0a7/internal/core-macros/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core-macros/LICENSES/GPL-3.0-only.txt` & `slint-1.6.0a7/internal/interpreter/LICENSES/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core-macros/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md` & `slint-1.6.0a7/internal/interpreter/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core-macros/LICENSES/LicenseRef-Slint-commercial.md` & `slint-1.6.0a7/internal/interpreter/LICENSES/LicenseRef-Slint-commercial.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core-macros/README.md` & `slint-1.6.0a7/internal/core-macros/README.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/core-macros/lib.rs` & `slint-1.6.0a7/internal/core-macros/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/interpreter/Cargo.toml` & `slint-1.6.0a7/internal/interpreter/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/interpreter/LICENSES/GPL-3.0-only.txt` & `slint-1.6.0a7/api/rs/slint/LICENSES/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/interpreter/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md` & `slint-1.6.0a7/api/rs/slint/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/interpreter/LICENSES/LicenseRef-Slint-commercial.md` & `slint-1.6.0a7/api/rs/slint/LICENSES/LicenseRef-Slint-commercial.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/interpreter/api.rs` & `slint-1.6.0a7/internal/interpreter/api.rs`

 * *Files 1% similar despite different names*

```diff
@@ -933,15 +933,15 @@
     }
 
     /// Return the value for a public property of this component.
     ///
     /// ## Examples
     ///
     /// ```
-    /// # i_slint_backend_testing::init();
+    /// # i_slint_backend_testing::init_no_event_loop();
     /// use slint_interpreter::{ComponentDefinition, ComponentCompiler, Value, SharedString};
     /// let code = r#"
     ///     export component MyWin inherits Window {
     ///         in-out property <int> my_property: 42;
     ///     }
     /// "#;
     /// let mut compiler = ComponentCompiler::default();
@@ -1000,15 +1000,15 @@
     /// Note: Since the [`ComponentInstance`] holds the handler, the handler itself should not
     /// contain a strong reference to the instance. So if you need to capture the instance,
     /// you should use [`Self::as_weak`] to create a weak reference.
     ///
     /// ## Examples
     ///
     /// ```
-    /// # i_slint_backend_testing::init();
+    /// # i_slint_backend_testing::init_no_event_loop();
     /// use slint_interpreter::{ComponentDefinition, ComponentCompiler, Value, SharedString, ComponentHandle};
     /// use core::convert::TryInto;
     /// let code = r#"
     ///     component MyWin inherits Window {
     ///         callback foo(int) -> int;
     ///         in-out property <int> my_prop: 12;
     ///     }
@@ -1056,15 +1056,15 @@
     ///
     /// The `global` parameter is the exported name of the global singleton. The `property` argument
     /// is the name of the property
     ///
     /// ## Examples
     ///
     /// ```
-    /// # i_slint_backend_testing::init();
+    /// # i_slint_backend_testing::init_no_event_loop();
     /// use slint_interpreter::{ComponentDefinition, ComponentCompiler, Value, SharedString};
     /// let code = r#"
     ///     global Glob {
     ///         in-out property <int> my_property: 42;
     ///     }
     ///     export { Glob as TheGlobal }
     ///     component MyWin inherits Window {
@@ -1111,15 +1111,15 @@
     /// Set a handler for the callback in the exported global singleton. A callback with that
     /// name must be defined in the specified global and the global must be exported from the
     /// main document otherwise an error will be returned.
     ///
     /// ## Examples
     ///
     /// ```
-    /// # i_slint_backend_testing::init();
+    /// # i_slint_backend_testing::init_no_event_loop();
     /// use slint_interpreter::{ComponentDefinition, ComponentCompiler, Value, SharedString};
     /// use core::convert::TryInto;
     /// let code = r#"
     ///     export global Logic {
     ///         pure callback to_uppercase(string) -> string;
     ///     }
     ///     component MyWin inherits Window {
@@ -1383,15 +1383,15 @@
             &WindowInner::from_pub(comp.window()).window_adapter(),
         );
     }
 }
 
 #[test]
 fn component_definition_properties() {
-    i_slint_backend_testing::init();
+    i_slint_backend_testing::init_no_event_loop();
     let mut compiler = ComponentCompiler::default();
     compiler.set_style("fluent".into());
     let comp_def = spin_on::spin_on(
         compiler.build_from_source(
             r#"
     export component Dummy {
         in-out property <string> test;
@@ -1431,15 +1431,15 @@
         Err(SetPropertyError::WrongType)
     );
     assert_eq!(instance.get_property("underscores-and-dashes-preserved"), Ok(Value::Number(88.)));
 }
 
 #[test]
 fn component_definition_properties2() {
-    i_slint_backend_testing::init();
+    i_slint_backend_testing::init_no_event_loop();
     let mut compiler = ComponentCompiler::default();
     compiler.set_style("fluent".into());
     let comp_def = spin_on::spin_on(
         compiler.build_from_source(
             r#"
     export component Dummy {
         in-out property <string> sub-text <=> sub.text;
@@ -1482,15 +1482,15 @@
 
     assert_eq!(instance.get_property("background"), Err(GetPropertyError::NoSuchProperty));
     assert_eq!(instance.get_property("xx"), Err(GetPropertyError::NoSuchProperty));
 }
 
 #[test]
 fn globals() {
-    i_slint_backend_testing::init();
+    i_slint_backend_testing::init_no_event_loop();
     let mut compiler = ComponentCompiler::default();
     compiler.set_style("fluent".into());
     let definition = spin_on::spin_on(
         compiler.build_from_source(
             r#"
     export global My-Super_Global {
         in-out property <int> the-property : 21;
@@ -1600,15 +1600,15 @@
         instance.invoke_global("My_Super_Global", "yoyo", &[]),
         Err(InvokeError::NoSuchCallable)
     );
 }
 
 #[test]
 fn call_functions() {
-    i_slint_backend_testing::init();
+    i_slint_backend_testing::init_no_event_loop();
     let mut compiler = ComponentCompiler::default();
     compiler.set_style("fluent".into());
     let definition = spin_on::spin_on(
         compiler.build_from_source(
             r#"
     export global Gl {
         out property<string> q;
@@ -1646,15 +1646,15 @@
         Ok(Value::String("Hello10".into()))
     );
     assert_eq!(instance.get_global_property("Gl", "q"), Ok(Value::String("Hello".into())));
 }
 
 #[test]
 fn component_definition_struct_properties() {
-    i_slint_backend_testing::init();
+    i_slint_backend_testing::init_no_event_loop();
     let mut compiler = ComponentCompiler::default();
     compiler.set_style("fluent".into());
     let comp_def = spin_on::spin_on(
         compiler.build_from_source(
             r#"
     export struct Settings {
         string_value: string,
@@ -1697,15 +1697,15 @@
         Err(SetPropertyError::WrongType)
     );
 }
 
 #[test]
 fn component_definition_model_properties() {
     use i_slint_core::model::*;
-    i_slint_backend_testing::init();
+    i_slint_backend_testing::init_no_event_loop();
     let mut compiler = ComponentCompiler::default();
     compiler.set_style("fluent".into());
     let comp_def = spin_on::spin_on(compiler.build_from_source(
         "export Dummy := Rectangle { property <[int]> prop: [42, 12]; }".into(),
         "".into(),
     ))
     .unwrap();
```

### Comparing `slint-1.6.0a6/internal/interpreter/dynamic_item_tree.rs` & `slint-1.6.0a7/internal/interpreter/dynamic_item_tree.rs`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 };
 use i_slint_core::items::{AccessibleRole, ItemRef, ItemVTable, PropertyAnimation};
 use i_slint_core::layout::{BoxLayoutCellData, LayoutInfo, Orientation};
 use i_slint_core::lengths::{LogicalLength, LogicalRect};
 use i_slint_core::model::RepeatedItemTree;
 use i_slint_core::model::Repeater;
 use i_slint_core::platform::PlatformError;
-use i_slint_core::properties::InterpolatedPropertyValue;
+use i_slint_core::properties::{ChangeTracker, InterpolatedPropertyValue};
 use i_slint_core::rtti::{self, AnimatedBindingKind, FieldOffset, PropertyInfo};
 use i_slint_core::slice::Slice;
 use i_slint_core::window::{WindowAdapterRc, WindowInner};
 use i_slint_core::{Brush, Color, Property, SharedString, SharedVector};
 use once_cell::unsync::OnceCell;
 use std::collections::BTreeMap;
 use std::collections::HashMap;
@@ -233,15 +233,15 @@
     }
 
     fn accessible_string_property(
         self: Pin<&Self>,
         index: u32,
         what: AccessibleStringProperty,
         result: &mut SharedString,
-    ) {
+    ) -> bool {
         self.borrow().as_ref().accessible_string_property(index, what, result)
     }
 
     fn window_adapter(self: Pin<&Self>, do_create: bool, result: &mut Option<WindowAdapterRc>) {
         self.borrow().as_ref().window_adapter(do_create, result);
     }
 
@@ -385,14 +385,18 @@
     pub(crate) extra_data_offset: FieldOffset<Instance<'id>, ComponentExtraData>,
     /// Keep the Rc alive
     pub(crate) original: Rc<object_tree::Component>,
     /// Maps from an item_id to the original element it came from
     pub(crate) original_elements: Vec<ElementRc>,
     /// Copy of original.root_element.property_declarations, without a guarded refcell
     public_properties: BTreeMap<String, PropertyDeclaration>,
+    change_trackers: Option<(
+        FieldOffset<Instance<'id>, OnceCell<Vec<ChangeTracker>>>,
+        Vec<(NamedReference, Expression)>,
+    )>,
 
     /// compiled globals
     compiled_globals: Vec<crate::global_component::CompiledGlobal>,
     /// Map of all exported global singletons and their index in the compiled_globals vector. The key
     /// is the normalized name of the global.
     exported_globals_by_name: BTreeMap<String, usize>,
 
@@ -896,14 +900,15 @@
             Vec<vtable::VOffset<crate::dynamic_type::Instance<'id>, ItemVTable, vtable::AllowPin>>,
         original_elements: Vec<ElementRc>,
         items_types: HashMap<String, ItemWithinItemTree>,
         type_builder: dynamic_type::TypeBuilder<'id>,
         repeater: Vec<ErasedRepeaterWithinComponent<'id>>,
         repeater_names: HashMap<String, usize>,
         rtti: Rc<HashMap<&'static str, Rc<ItemRTTI>>>,
+        change_callbacks: Vec<(NamedReference, Expression)>,
     }
     impl<'id> generator::ItemTreeBuilder for TreeBuilder<'id> {
         type SubComponentState = ();
 
         fn push_repeated_item(
             &mut self,
             item_rc: &ElementRc,
@@ -963,14 +968,20 @@
             self.item_array.push(unsafe { vtable::VOffset::from_raw(rt.vtable, offset) });
             self.original_elements.push(rc_item.clone());
             debug_assert_eq!(self.original_elements.len(), self.tree_array.len());
             self.items_types.insert(
                 item.id.clone(),
                 ItemWithinItemTree { offset, rtti: rt.clone(), elem: rc_item.clone() },
             );
+            for (prop, expr) in &item.change_callbacks {
+                self.change_callbacks.push((
+                    NamedReference::new(&rc_item, prop),
+                    Expression::CodeBlock(expr.borrow().clone()),
+                ));
+            }
         }
 
         fn enter_component(
             &mut self,
             _item: &ElementRc,
             _sub_component: &Rc<object_tree::Component>,
             _children_offset: u32,
@@ -995,14 +1006,15 @@
         item_array: vec![],
         original_elements: vec![],
         items_types: HashMap::new(),
         type_builder: dynamic_type::TypeBuilder::new(guard),
         repeater: vec![],
         repeater_names: HashMap::new(),
         rtti: Rc::new(rtti),
+        change_callbacks: vec![],
     };
 
     if !component.is_global() {
         generator::build_item_tree(component, &(), &mut builder);
     }
 
     let mut custom_properties = HashMap::new();
@@ -1124,14 +1136,21 @@
 
     let root_offset = builder.type_builder.add_field_type::<OnceCell<ErasedItemTreeBoxWeak>>();
 
     let window_adapter_offset = builder.type_builder.add_field_type::<OnceCell<WindowAdapterRc>>();
 
     let extra_data_offset = builder.type_builder.add_field_type::<ComponentExtraData>();
 
+    let change_trackers = (!builder.change_callbacks.is_empty()).then(|| {
+        (
+            builder.type_builder.add_field_type::<OnceCell<Vec<ChangeTracker>>>(),
+            builder.change_callbacks,
+        )
+    });
+
     let public_properties = component.root_element.borrow().property_declarations.clone();
 
     let mut exported_globals_by_name: BTreeMap<String, usize> = Default::default();
 
     let compiled_globals = component
         .used_types
         .borrow()
@@ -1193,14 +1212,15 @@
         parent_item_tree_offset,
         root_offset,
         window_adapter_offset,
         extra_data_offset,
         public_properties,
         compiled_globals,
         exported_globals_by_name,
+        change_trackers,
         #[cfg(feature = "highlight")]
         type_loader: std::cell::OnceCell::new(),
     };
 
     Rc::new(t)
 }
 
@@ -1604,14 +1624,52 @@
         let instance_ref = compo_box.borrow_instance();
         for extra_init_code in self.0.description.original.init_code.borrow().iter() {
             eval::eval_expression(
                 extra_init_code,
                 &mut eval::EvalLocalContext::from_component_instance(instance_ref),
             );
         }
+        if let Some(cts) = instance_ref.description.change_trackers.as_ref() {
+            let self_weak = instance_ref.self_weak().get().unwrap();
+            let v = cts
+                .1
+                .iter()
+                .enumerate()
+                .map(|(idx, _)| {
+                    let ct = ChangeTracker::default();
+                    ct.init(
+                        self_weak.clone(),
+                        move |self_weak| {
+                            let s = self_weak.upgrade().unwrap();
+                            generativity::make_guard!(guard);
+                            let compo_box = s.unerase(guard);
+                            let instance_ref = compo_box.borrow_instance();
+                            let nr = &s.0.description.change_trackers.as_ref().unwrap().1[idx].0;
+                            eval::load_property(instance_ref, &nr.element(), nr.name()).unwrap()
+                        },
+                        move |self_weak, _| {
+                            let s = self_weak.upgrade().unwrap();
+                            generativity::make_guard!(guard);
+                            let compo_box = s.unerase(guard);
+                            let instance_ref = compo_box.borrow_instance();
+                            let e = &s.0.description.change_trackers.as_ref().unwrap().1[idx].1;
+                            eval::eval_expression(
+                                e,
+                                &mut eval::EvalLocalContext::from_component_instance(instance_ref),
+                            );
+                        },
+                    );
+                    ct
+                })
+                .collect::<Vec<_>>();
+            cts.0
+                .apply_pin(instance_ref.instance)
+                .set(v)
+                .unwrap_or_else(|_| panic!("run_setup_code called twice?"));
+        }
     }
 }
 impl<'id> From<ItemTreeBox<'id>> for ErasedItemTreeBox {
     fn from(inner: ItemTreeBox<'id>) -> Self {
         // Safety: Nothing access the component directly, we only access it through unerased where
         // the lifetime is unique again
         unsafe {
@@ -1867,15 +1925,15 @@
 }
 
 extern "C" fn accessible_string_property(
     component: ItemTreeRefPin,
     item_index: u32,
     what: AccessibleStringProperty,
     result: &mut SharedString,
-) {
+) -> bool {
     generativity::make_guard!(guard);
     let instance_ref = unsafe { InstanceRef::from_pin_ref(component, guard) };
     let prop_name = format!("accessible-{}", what);
     let nr = instance_ref.description.original_elements[item_index as usize]
         .borrow()
         .accessibility_props
         .0
@@ -1885,14 +1943,17 @@
         let value = crate::eval::load_property(instance_ref, &nr.element(), nr.name()).unwrap();
         match value {
             Value::String(s) => *result = s,
             Value::Bool(b) => *result = if b { "true" } else { "false" }.into(),
             Value::Number(x) => *result = x.to_string().into(),
             _ => unimplemented!("invalid type for accessible_string_property"),
         };
+        true
+    } else {
+        false
     }
 }
 
 extern "C" fn accessibility_action(
     component: ItemTreeRefPin,
     item_index: u32,
     action: &AccessibilityAction,
```

### Comparing `slint-1.6.0a6/internal/interpreter/dynamic_type.rs` & `slint-1.6.0a7/internal/interpreter/dynamic_type.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/interpreter/eval.rs` & `slint-1.6.0a7/internal/interpreter/eval.rs`

 * *Files 1% similar despite different names*

```diff
@@ -523,24 +523,64 @@
 
                 let item_info = &description.items[focus_item.borrow().id.as_str()];
 
                 let focus_item_comp =
                     enclosing_component.self_weak().get().unwrap().upgrade().unwrap();
 
                 component.access_window(|window| {
-                    window.set_focus_item(&corelib::items::ItemRc::new(
-                        vtable::VRc::into_dyn(focus_item_comp),
-                        item_info.item_index(),
-                    ))
+                    window.set_focus_item(
+                        &corelib::items::ItemRc::new(
+                            vtable::VRc::into_dyn(focus_item_comp),
+                            item_info.item_index(),
+                        ),
+                        true,
+                    )
                 });
                 Value::Void
             } else {
                 panic!("internal error: argument to SetFocusItem must be an element")
             }
         }
+        BuiltinFunction::ClearFocusItem => {
+            if arguments.len() != 1 {
+                panic!("internal error: incorrect argument count to SetFocusItem")
+            }
+            let component = match local_context.component_instance {
+                ComponentInstance::InstanceRef(c) => c,
+                ComponentInstance::GlobalComponent(_) => {
+                    panic!("Cannot access the focus item from a global component")
+                }
+            };
+            if let Expression::ElementReference(focus_item) = &arguments[0] {
+                generativity::make_guard!(guard);
+
+                let focus_item = focus_item.upgrade().unwrap();
+                let enclosing_component =
+                    enclosing_component_for_element(&focus_item, component, guard);
+                let description = enclosing_component.description;
+
+                let item_info = &description.items[focus_item.borrow().id.as_str()];
+
+                let focus_item_comp =
+                    enclosing_component.self_weak().get().unwrap().upgrade().unwrap();
+
+                component.access_window(|window| {
+                    window.set_focus_item(
+                        &corelib::items::ItemRc::new(
+                            vtable::VRc::into_dyn(focus_item_comp),
+                            item_info.item_index(),
+                        ),
+                        false,
+                    )
+                });
+                Value::Void
+            } else {
+                panic!("internal error: argument to ClearFocusItem must be an element")
+            }
+        }
         BuiltinFunction::ShowPopupWindow => {
             if arguments.len() != 1 {
                 panic!("internal error: incorrect argument count to ShowPopupWindow")
             }
             let component = match local_context.component_instance {
                 ComponentInstance::InstanceRef(c) => c,
                 ComponentInstance::GlobalComponent(_) => {
```

### Comparing `slint-1.6.0a6/internal/interpreter/eval_layout.rs` & `slint-1.6.0a7/internal/interpreter/eval_layout.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/interpreter/ffi.rs` & `slint-1.6.0a7/internal/interpreter/ffi.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/interpreter/global_component.rs` & `slint-1.6.0a7/internal/interpreter/global_component.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/interpreter/highlight.rs` & `slint-1.6.0a7/internal/interpreter/highlight.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/interpreter/lib.rs` & `slint-1.6.0a7/internal/interpreter/lib.rs`

 * *Files 7% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     instance.run().unwrap();
 }
 ```
 
 This example load a `.slint` from a string and set some properties:
 
 ```rust
-# i_slint_backend_testing::init();
+# i_slint_backend_testing::init_no_event_loop();
 use slint_interpreter::{ComponentDefinition, ComponentCompiler, Value, SharedString, ComponentHandle};
 
 let code = r#"
     export component MyWin inherits Window {
         in property <string> my_name;
         Text {
             text: "Hello, " + my_name;
```

### Comparing `slint-1.6.0a6/internal/interpreter/migration.rs` & `slint-1.6.0a7/internal/interpreter/migration.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/interpreter/tests.rs` & `slint-1.6.0a7/internal/interpreter/tests.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 // Copyright © SixtyFPS GmbH <info@slint.dev>
 // SPDX-License-Identifier: GPL-3.0-only OR LicenseRef-Slint-Royalty-free-1.2 OR LicenseRef-Slint-commercial
 
 #[cfg(feature = "internal")]
 #[test]
 fn reuse_window() {
-    i_slint_backend_testing::init();
+    i_slint_backend_testing::init_no_event_loop();
     use crate::{ComponentCompiler, ComponentHandle, SharedString, Value};
     let code = r#"
         export component MainWindow inherits Window {
             in-out property<string> text_text: "foo";
             in-out property<string> text_alias: input.text;
             input := TextInput {
                 text:  self.enabled ? text_text : text_text;
```

### Comparing `slint-1.6.0a6/internal/interpreter/value_model.rs` & `slint-1.6.0a7/internal/interpreter/value_model.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/helper_crates/vtable/macro/Cargo.toml` & `slint-1.6.0a7/helper_crates/vtable/macro/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/helper_crates/vtable/macro/LICENSES/Apache-2.0.txt` & `slint-1.6.0a7/helper_crates/const-field-offset/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/helper_crates/vtable/macro/LICENSES/MIT.txt` & `slint-1.6.0a7/helper_crates/vtable/macro/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/helper_crates/vtable/macro/macro.rs` & `slint-1.6.0a7/helper_crates/vtable/macro/macro.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/qt/Cargo.toml` & `slint-1.6.0a7/internal/backends/qt/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/qt/LICENSES/GPL-3.0-only.txt` & `slint-1.6.0a7/internal/backends/android-activity/LICENSES/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/qt/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md` & `slint-1.6.0a7/internal/backends/android-activity/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/qt/LICENSES/LicenseRef-Slint-commercial.md` & `slint-1.6.0a7/internal/backends/android-activity/LICENSES/LicenseRef-Slint-commercial.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/qt/accessible_generated.rs` & `slint-1.6.0a7/internal/backends/qt/accessible_generated.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/qt/build.rs` & `slint-1.6.0a7/internal/backends/qt/build.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/qt/key_generated.rs` & `slint-1.6.0a7/internal/backends/qt/key_generated.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/qt/lib.rs` & `slint-1.6.0a7/internal/backends/qt/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/qt/qt_accessible.rs` & `slint-1.6.0a7/internal/backends/qt/qt_accessible.rs`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 const CHECKABLE: u32 = VALUE_STEP + 1;
 
 pub struct AccessibleItemPropertiesTracker {
     obj: *mut c_void,
 }
 
 impl PropertyDirtyHandler for AccessibleItemPropertiesTracker {
-    fn notify(&self) {
+    fn notify(self: Pin<&Self>) {
         let obj = self.obj;
         cpp!(unsafe [obj as "QObject*"] {
             QTimer::singleShot(0, [obj = QPointer(obj)]() {
                 if (!obj)
                     return;
 
                 auto accessible_item = static_cast<Slint_accessible_item*>(QAccessible::queryAccessibleInterface(obj));
@@ -59,15 +59,15 @@
 }
 
 pub struct ValuePropertyTracker {
     obj: *mut c_void,
 }
 
 impl PropertyDirtyHandler for ValuePropertyTracker {
-    fn notify(&self) {
+    fn notify(self: Pin<&Self>) {
         let obj = self.obj;
         cpp!(unsafe [obj as "QObject*"] {
             QTimer::singleShot(0, [ obj = QPointer(obj)]() {
                 if (!obj)
                     return;
 
                 auto accessible_item = static_cast<Slint_accessible_item*>(QAccessible::queryAccessibleInterface(obj));
@@ -84,15 +84,15 @@
 }
 
 pub struct LabelPropertyTracker {
     obj: *mut c_void,
 }
 
 impl PropertyDirtyHandler for LabelPropertyTracker {
-    fn notify(&self) {
+    fn notify(self: Pin<&Self>) {
         let obj = self.obj;
         cpp!(unsafe [obj as "QObject*"] {
             QTimer::singleShot(0, [obj = QPointer(obj)]() {
                 if (!obj)
                     return;
 
                 auto accessible_item = static_cast<Slint_accessible_item*>(QAccessible::queryAccessibleInterface(obj));
@@ -109,15 +109,15 @@
 }
 
 pub struct DescriptionPropertyTracker {
     obj: *mut c_void,
 }
 
 impl PropertyDirtyHandler for DescriptionPropertyTracker {
-    fn notify(&self) {
+    fn notify(self: Pin<&Self>) {
         let obj = self.obj;
         cpp!(unsafe [obj as "QObject*"] {
             QTimer::singleShot(0, [obj = QPointer(obj)]() {
                 if (!obj)
                     return;
 
                 auto accessible_item = static_cast<Slint_accessible_item*>(QAccessible::queryAccessibleInterface(obj));
@@ -134,15 +134,15 @@
 }
 
 pub struct FocusDelegationPropertyTracker {
     obj: *mut c_void,
 }
 
 impl PropertyDirtyHandler for FocusDelegationPropertyTracker {
-    fn notify(&self) {
+    fn notify(self: Pin<&Self>) {
         let obj = self.obj;
         cpp!(unsafe [obj as "QObject*"] {
             QTimer::singleShot(0, [obj = QPointer(obj)]() {
                 if (!obj)
                     return;
 
                 auto accessible_item = static_cast<Slint_accessible_item*>(QAccessible::queryAccessibleInterface(obj));
@@ -354,20 +354,21 @@
                     DESCRIPTION => item.accessible_string_property(AccessibleStringProperty::Description),
                     VALUE => item.accessible_string_property(AccessibleStringProperty::Value),
                     CHECKED => item.accessible_string_property(AccessibleStringProperty::Checked),
                     VALUE_MINIMUM => item.accessible_string_property(AccessibleStringProperty::ValueMinimum),
                     VALUE_MAXIMUM => item.accessible_string_property(AccessibleStringProperty::ValueMaximum),
                     VALUE_STEP => item.accessible_string_property(AccessibleStringProperty::ValueStep),
                     CHECKABLE => item.accessible_string_property(AccessibleStringProperty::Checkable),
-                    _ => Default::default(),
+                    _ => None,
                 };
-                QString::from(string.as_ref())
-            } else {
-                QString::default()
-            }
+                if let Some(string) = string {
+                    return QString::from(string.as_ref())
+                }
+            };
+            QString::default()
         });
     }
 
     // ------------------------------------------------------------------------------
     // Slint_accessible:
     // ------------------------------------------------------------------------------
 
@@ -587,15 +588,15 @@
         }
 
         void delegateFocus() const override {
             if (!has_focus) { return; }
 
             auto index = rust!(Slint_accessible_item_delegate_focus [m_data: Pin<&SlintAccessibleItemData> as "void*"] -> i32 as "int" {
                 m_data.item.upgrade()
-                    .map(|i| { i.accessible_string_property(AccessibleStringProperty::DelegateFocus) })
+                    .and_then(|i| { i.accessible_string_property(AccessibleStringProperty::DelegateFocus) })
                     .and_then(|s| s.as_str().parse::<i32>().ok()).unwrap_or(-1)
             });
 
             if (index >= 0 && index < rawChildCount()) {
                 static_cast<Slint_accessible_item*>(rawChild(index))->sendFocusChangeEvent();
             } else {
                 sendFocusChangeEvent();
```

### Comparing `slint-1.6.0a6/internal/backends/qt/qt_widgets/button.rs` & `slint-1.6.0a7/internal/backends/qt/qt_widgets/button.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/qt/qt_widgets/checkbox.rs` & `slint-1.6.0a7/internal/backends/qt/qt_widgets/checkbox.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/qt/qt_widgets/combobox.rs` & `slint-1.6.0a7/internal/backends/qt/qt_widgets/combobox.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/qt/qt_widgets/groupbox.rs` & `slint-1.6.0a7/internal/backends/qt/qt_widgets/groupbox.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/qt/qt_widgets/lineedit.rs` & `slint-1.6.0a7/internal/backends/qt/qt_widgets/lineedit.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/qt/qt_widgets/listviewitem.rs` & `slint-1.6.0a7/internal/backends/qt/qt_widgets/listviewitem.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/qt/qt_widgets/palette.rs` & `slint-1.6.0a7/internal/backends/qt/qt_widgets/palette.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/qt/qt_widgets/progress_indicator.rs` & `slint-1.6.0a7/internal/backends/qt/qt_widgets/progress_indicator.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/qt/qt_widgets/scrollview.rs` & `slint-1.6.0a7/internal/backends/qt/qt_widgets/scrollview.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/qt/qt_widgets/slider.rs` & `slint-1.6.0a7/internal/backends/qt/qt_widgets/slider.rs`

 * *Files 0% similar despite different names*

```diff
@@ -205,15 +205,15 @@
             }
             MouseEvent::Pressed {
                 position: pos,
                 button: PointerEventButton::Left,
                 click_count: _,
             } => {
                 if !self.has_focus() {
-                    WindowInner::from_pub(window_adapter.window()).set_focus_item(self_rc);
+                    WindowInner::from_pub(window_adapter.window()).set_focus_item(self_rc, true);
                 }
                 data.pressed_x = if vertical { pos.y as f32 } else { pos.x as f32 };
                 data.pressed = 1;
                 data.pressed_val = self.value();
                 InputEventResult::GrabMouse
             }
             MouseEvent::Exit | MouseEvent::Released { button: PointerEventButton::Left, .. } => {
```

### Comparing `slint-1.6.0a6/internal/backends/qt/qt_widgets/spinbox.rs` & `slint-1.6.0a7/internal/backends/qt/qt_widgets/spinbox.rs`

 * *Files 1% similar despite different names*

```diff
@@ -218,15 +218,15 @@
         data.active_controls = new_control;
         if changed {
             self.data.set(data);
         }
 
         if let MouseEvent::Pressed { .. } = event {
             if !self.has_focus() {
-                WindowInner::from_pub(window_adapter.window()).set_focus_item(self_rc);
+                WindowInner::from_pub(window_adapter.window()).set_focus_item(self_rc, true);
             }
         }
         InputEventResult::EventAccepted
     }
 
     fn key_event(
         self: Pin<&Self>,
```

### Comparing `slint-1.6.0a6/internal/backends/qt/qt_widgets/stylemetrics.rs` & `slint-1.6.0a7/internal/backends/qt/qt_widgets/stylemetrics.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/qt/qt_widgets/tableheadersection.rs` & `slint-1.6.0a7/internal/backends/qt/qt_widgets/tableheadersection.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/qt/qt_widgets/tabwidget.rs` & `slint-1.6.0a7/internal/backends/qt/qt_widgets/tabwidget.rs`

 * *Files 0% similar despite different names*

```diff
@@ -436,15 +436,15 @@
         });
         let click_on_press = cpp!(unsafe [] -> bool as "bool" {
             return qApp->style()->styleHint(QStyle::SH_TabBar_SelectMouseType, nullptr, nullptr) == QEvent::MouseButtonPress;
         });
         if matches!(event, MouseEvent::Released { button, .. } if !click_on_press && button == PointerEventButton::Left)
             || matches!(event, MouseEvent::Pressed { button, .. } if click_on_press && button == PointerEventButton::Left)
         {
-            WindowInner::from_pub(window_adapter.window()).set_focus_item(self_rc);
+            WindowInner::from_pub(window_adapter.window()).set_focus_item(self_rc, true);
             self.current.set(self.tab_index());
             InputEventResult::EventAccepted
         } else {
             InputEventResult::GrabMouse
         }
     }
```

### Comparing `slint-1.6.0a6/internal/backends/qt/qt_widgets.rs` & `slint-1.6.0a7/internal/backends/qt/qt_widgets.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/qt/qt_window.rs` & `slint-1.6.0a7/internal/backends/qt/qt_window.rs`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 use i_slint_core::input::{KeyEvent, KeyEventType, MouseEvent};
 use i_slint_core::item_rendering::{
     CachedRenderingData, ItemCache, ItemRenderer, RenderBorderRectangle, RenderImage,
 };
 use i_slint_core::item_tree::{ItemTreeRc, ItemTreeRef};
 use i_slint_core::items::{
     self, ColorScheme, FillRule, ImageRendering, ItemRc, ItemRef, Layer, MouseCursor, Opacity,
-    PointerEventButton, RenderingResult, TextOverflow, TextWrap,
+    PointerEventButton, RenderingResult, TextOverflow, TextStrokeStyle, TextWrap,
 };
 use i_slint_core::layout::Orientation;
 use i_slint_core::lengths::{
     LogicalBorderRadius, LogicalLength, LogicalPoint, LogicalRect, LogicalSize, LogicalVector,
     PhysicalPx, ScaleFactor,
 };
 use i_slint_core::platform::{PlatformError, WindowEvent};
@@ -660,55 +660,56 @@
     ) {
         self.draw_image_impl(item_rc, size, image);
     }
 
     fn draw_text(&mut self, text: std::pin::Pin<&items::Text>, _: &ItemRc, size: LogicalSize) {
         let rect: qttypes::QRectF = check_geometry!(size);
         let fill_brush: qttypes::QBrush = into_qbrush(text.color(), rect.width, rect.height);
+        let stroke_brush: qttypes::QBrush = into_qbrush(text.stroke(), rect.width, rect.height);
         let mut string: qttypes::QString = text.text().as_str().into();
         let font: QFont = get_font(text.font_request(WindowInner::from_pub(self.window)));
-        let flags = match text.horizontal_alignment() {
+        let alignment = match text.horizontal_alignment() {
             TextHorizontalAlignment::Left => key_generated::Qt_AlignmentFlag_AlignLeft,
             TextHorizontalAlignment::Center => key_generated::Qt_AlignmentFlag_AlignHCenter,
             TextHorizontalAlignment::Right => key_generated::Qt_AlignmentFlag_AlignRight,
         } | match text.vertical_alignment() {
             TextVerticalAlignment::Top => key_generated::Qt_AlignmentFlag_AlignTop,
             TextVerticalAlignment::Center => key_generated::Qt_AlignmentFlag_AlignVCenter,
             TextVerticalAlignment::Bottom => key_generated::Qt_AlignmentFlag_AlignBottom,
-        } | match text.wrap() {
-            TextWrap::NoWrap => 0,
-            TextWrap::WordWrap => key_generated::Qt_TextFlag_TextWordWrap,
         };
+        let wrap = text.wrap() == TextWrap::WordWrap;
         let elide = text.overflow() == TextOverflow::Elide;
+        let stroke_visible = !text.stroke().is_transparent();
+        let stroke_outside = text.stroke_style() == TextStrokeStyle::Outside;
+        let stroke_width = match text.stroke_style() {
+            TextStrokeStyle::Outside => text.stroke_width().get() * 2.0,
+            TextStrokeStyle::Center => text.stroke_width().get(),
+        };
         let painter: &mut QPainterPtr = &mut self.painter;
-        cpp! { unsafe [painter as "QPainterPtr*", rect as "QRectF", fill_brush as "QBrush", mut string as "QString", flags as "int", font as "QFont", elide as "bool"] {
-            (*painter)->setFont(font);
-            (*painter)->setPen(QPen(fill_brush, 0));
-            (*painter)->setBrush(Qt::NoBrush);
+        cpp! { unsafe [painter as "QPainterPtr*", rect as "QRectF", fill_brush as "QBrush", stroke_brush as "QBrush", mut string as "QString", font as "QFont", elide as "bool", alignment as "Qt::Alignment", wrap as "bool", stroke_visible as "bool", stroke_outside as "bool", stroke_width as "float"] {
+            QString elided;
             if (!elide) {
-                (*painter)->drawText(rect, flags, string);
-            } else if (!(flags & Qt::TextWordWrap)) {
-                QString elided;
+                elided = string;
+            } else if (!wrap) {
                 QFontMetrics fm(font);
                 while (!string.isEmpty()) {
                     int pos = string.indexOf('\n');
                     if (pos < 0) {
                         elided += fm.elidedText(string, Qt::ElideRight, rect.width());
                         break;
                     }
                     QString line = string.left(pos);
                     elided += fm.elidedText(line, Qt::ElideRight, rect.width());
                     elided += '\n';
                     string = string.mid(pos + 1);
                 }
-                (*painter)->drawText(rect, flags, elided);
             } else {
                 // elide and word wrap: we need to add the ellipsis manually on the last line
                 string.replace(QChar('\n'), QChar::LineSeparator);
-                QString elided = string;
+                elided = string;
                 QFontMetrics fm(font);
                 QTextLayout layout(string, font);
                 QTextOption options;
                 options.setWrapMode(QTextOption::WordWrap);
                 layout.setTextOption(options);
                 layout.setCacheEnabled(true);
                 layout.beginLayout();
@@ -730,15 +731,90 @@
                     last_line_size = line.textLength();
                 }
                 if (last_line_begin < string.size()) {
                     elided = string.left(last_line_begin);
                     QString to_elide = QStringView(string).mid(last_line_begin, last_line_size).trimmed() % QStringView(QT_UNICODE_LITERAL("…"));
                     elided += fm.elidedText(to_elide, Qt::ElideRight, rect.width());
                 }
+            }
+
+            if (!stroke_visible) {
+                int flags = alignment;
+                if (wrap)
+                    flags |= Qt::TextWordWrap;
+
+                (*painter)->setFont(font);
+                (*painter)->setBrush(Qt::NoBrush);
+                (*painter)->setPen(QPen(fill_brush, 0));
                 (*painter)->drawText(rect, flags, elided);
+            } else {
+                QTextDocument document(elided);
+                document.setDocumentMargin(0);
+                document.setPageSize(rect.size());
+                document.setDefaultFont(font);
+
+                QTextOption options = document.defaultTextOption();
+                options.setAlignment(alignment);
+                if (wrap)
+                    options.setWrapMode(QTextOption::WordWrap);
+                document.setDefaultTextOption(options);
+
+                // Workaround for https://bugreports.qt.io/browse/QTBUG-13467
+                float dy = 0;
+                if (!(alignment & Qt::AlignTop)) {
+                    QRectF bounding_rect;
+                    for (QTextBlock it = document.begin(); it != document.end(); it = it.next()) {
+                        bounding_rect = bounding_rect.united(document.documentLayout()->blockBoundingRect(it));
+                    }
+                    if (alignment & Qt::AlignVCenter) {
+                        dy = (rect.height() - bounding_rect.height()) / 2.0;
+                    } else if (alignment & Qt::AlignBottom) {
+                        dy = (rect.height() - bounding_rect.height());
+                    }
+                }
+
+                QTextCharFormat format;
+                format.setFont(font);
+
+                QPen stroke_pen(stroke_brush, stroke_width, Qt::SolidLine, Qt::FlatCap, Qt::MiterJoin);
+                stroke_pen.setMiterLimit(10.0);
+                if (stroke_width == 0.0) {
+                    // Hairline stroke
+                    if (stroke_outside)
+                        stroke_pen.setWidthF(2.0);
+                    else
+                        stroke_pen.setWidthF(1.0);
+                    stroke_pen.setCosmetic(true);
+                }
+
+                QTextCursor cursor(&document);
+                cursor.select(QTextCursor::Document);
+
+                (*painter)->save();
+                (*painter)->translate(0, dy);
+
+                if (stroke_outside) {
+                    format.setForeground(Qt::NoBrush);
+                    format.setTextOutline(stroke_pen);
+                    cursor.mergeCharFormat(format);
+                    document.drawContents((*painter).get(), rect);
+                }
+
+                format.setForeground(fill_brush);
+                if (!stroke_outside) {
+                    format.setTextOutline(stroke_pen);
+                } else {
+                    // Use a transparent pen instead of Qt::NoPen so the
+                    // fill is aligned properly to the outside stroke
+                    format.setTextOutline(QPen(QColor(Qt::transparent), stroke_width));
+                }
+                cursor.mergeCharFormat(format);
+                document.drawContents((*painter).get(), rect);
+
+                (*painter)->restore();
             }
         }}
     }
 
     fn draw_text_input(
         &mut self,
         text_input: std::pin::Pin<&items::TextInput>,
```

### Comparing `slint-1.6.0a6/internal/renderers/femtovg/Cargo.toml` & `slint-1.6.0a7/internal/renderers/femtovg/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/renderers/femtovg/LICENSES/GPL-3.0-only.txt` & `slint-1.6.0a7/api/rs/build/LICENSES/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/renderers/femtovg/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md` & `slint-1.6.0a7/api/rs/build/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/renderers/femtovg/LICENSES/LicenseRef-Slint-commercial.md` & `slint-1.6.0a7/api/rs/build/LICENSES/LicenseRef-Slint-commercial.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/renderers/femtovg/fonts.rs` & `slint-1.6.0a7/internal/renderers/femtovg/fonts.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/renderers/femtovg/images.rs` & `slint-1.6.0a7/internal/renderers/femtovg/images.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/renderers/femtovg/itemrenderer.rs` & `slint-1.6.0a7/internal/renderers/femtovg/itemrenderer.rs`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 use i_slint_core::graphics::rendering_metrics_collector::RenderingMetrics;
 use i_slint_core::graphics::{IntRect, Point, Size};
 use i_slint_core::item_rendering::{
     CachedRenderingData, ItemCache, ItemRenderer, RenderBorderRectangle, RenderImage,
 };
 use i_slint_core::items::{
     self, Clip, FillRule, ImageRendering, ItemRc, Layer, Opacity, RenderingResult,
-    TextHorizontalAlignment,
+    TextHorizontalAlignment, TextStrokeStyle,
 };
 use i_slint_core::lengths::{
     LogicalBorderRadius, LogicalLength, LogicalPoint, LogicalRect, LogicalSize, LogicalVector,
     PointLengths, RectLengths, ScaleFactor, SizeLengths,
 };
 use i_slint_core::window::WindowInner;
 use i_slint_core::{Brush, Color, ImageInner, SharedString};
@@ -312,33 +312,67 @@
             cache.borrow_mut().font(
                 text.font_request(WindowInner::from_pub(self.window)),
                 self.scale_factor,
                 &text.text(),
             )
         });
 
-        let paint = match self
-            .brush_to_paint(text.color(), &rect_to_path((size * self.scale_factor).into()))
-        {
+        let text_path = rect_to_path((size * self.scale_factor).into());
+        let paint = match self.brush_to_paint(text.color(), &text_path) {
             Some(paint) => font.init_paint(text.letter_spacing() * self.scale_factor, paint),
             None => return,
         };
 
+        let stroke_style = text.stroke_style();
+        let stroke_width = if text.stroke_width().get() != 0.0 {
+            (text.stroke_width() * self.scale_factor).get()
+        } else {
+            // Hairline stroke
+            1.0
+        };
+        let stroke_width = match stroke_style {
+            TextStrokeStyle::Outside => stroke_width * 2.0,
+            TextStrokeStyle::Center => stroke_width,
+        };
+        let stroke_paint = match self.brush_to_paint(text.stroke(), &text_path) {
+            Some(mut paint) => {
+                if text.stroke().is_transparent() {
+                    None
+                } else {
+                    paint.set_line_width(stroke_width);
+                    Some(font.init_paint(text.letter_spacing() * self.scale_factor, paint))
+                }
+            }
+            None => None,
+        };
+
         let mut canvas = self.canvas.borrow_mut();
         fonts::layout_text_lines(
             string,
             &font,
             PhysicalSize::from_lengths(max_width, max_height),
             (text.horizontal_alignment(), text.vertical_alignment()),
             text.wrap(),
             text.overflow(),
             false,
             &paint,
             |to_draw, pos, _, _| {
-                canvas.fill_text(pos.x, pos.y, to_draw.trim_end(), &paint).unwrap();
+                match (stroke_style, &stroke_paint) {
+                    (TextStrokeStyle::Outside, Some(stroke_paint)) => {
+                        canvas.stroke_text(pos.x, pos.y, to_draw.trim_end(), stroke_paint).unwrap();
+                        canvas.fill_text(pos.x, pos.y, to_draw.trim_end(), &paint).unwrap();
+                    }
+                    (TextStrokeStyle::Center, Some(stroke_paint)) => {
+                        canvas.fill_text(pos.x, pos.y, to_draw.trim_end(), &paint).unwrap();
+                        canvas.stroke_text(pos.x, pos.y, to_draw.trim_end(), stroke_paint).unwrap();
+                    }
+                    _ => {
+                        canvas.fill_text(pos.x, pos.y, to_draw.trim_end(), &paint).unwrap();
+                    }
+                };
             },
         );
     }
 
     fn draw_text_input(
         &mut self,
         text_input: Pin<&items::TextInput>,
```

### Comparing `slint-1.6.0a6/internal/renderers/femtovg/lib.rs` & `slint-1.6.0a7/internal/renderers/femtovg/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/helper_crates/vtable/Cargo.toml` & `slint-1.6.0a7/helper_crates/vtable/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/helper_crates/vtable/CHANGELOG.md` & `slint-1.6.0a7/helper_crates/vtable/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/helper_crates/vtable/LICENSES/Apache-2.0.txt` & `slint-1.6.0a7/helper_crates/vtable/macro/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/helper_crates/vtable/LICENSES/MIT.txt` & `slint-1.6.0a7/helper_crates/vtable/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/helper_crates/vtable/src/compile_fail_tests.rs` & `slint-1.6.0a7/helper_crates/vtable/src/compile_fail_tests.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/helper_crates/vtable/src/lib.rs` & `slint-1.6.0a7/helper_crates/vtable/src/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/helper_crates/vtable/src/vrc.rs` & `slint-1.6.0a7/helper_crates/vtable/src/vrc.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/helper_crates/vtable/tests/test_vrc.rs` & `slint-1.6.0a7/helper_crates/vtable/tests/test_vrc.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/helper_crates/vtable/tests/test_vtable.rs` & `slint-1.6.0a7/helper_crates/vtable/tests/test_vtable.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/build/Cargo.toml` & `slint-1.6.0a7/api/rs/build/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/build/LICENSES/GPL-3.0-only.txt` & `slint-1.6.0a7/internal/backends/qt/LICENSES/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/build/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md` & `slint-1.6.0a7/internal/backends/qt/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/build/LICENSES/LicenseRef-Slint-commercial.md` & `slint-1.6.0a7/internal/backends/qt/LICENSES/LicenseRef-Slint-commercial.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/rs/build/lib.rs` & `slint-1.6.0a7/api/rs/build/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/selector/Cargo.toml` & `slint-1.6.0a7/internal/backends/selector/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/selector/LICENSES/GPL-3.0-only.txt` & `slint-1.6.0a7/internal/core-macros/LICENSES/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/selector/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md` & `slint-1.6.0a7/internal/core-macros/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/selector/LICENSES/LicenseRef-Slint-commercial.md` & `slint-1.6.0a7/internal/core-macros/LICENSES/LicenseRef-Slint-commercial.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/selector/README.md` & `slint-1.6.0a7/internal/backends/selector/README.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/selector/build.rs` & `slint-1.6.0a7/internal/backends/selector/build.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/internal/backends/selector/lib.rs` & `slint-1.6.0a7/internal/backends/selector/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/helper_crates/const-field-offset/Cargo.toml` & `slint-1.6.0a7/helper_crates/const-field-offset/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/helper_crates/const-field-offset/CHANGELOG.md` & `slint-1.6.0a7/helper_crates/const-field-offset/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/helper_crates/const-field-offset/LICENSES/Apache-2.0.txt` & `slint-1.6.0a7/helper_crates/vtable/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/helper_crates/const-field-offset/LICENSES/MIT.txt` & `slint-1.6.0a7/api/rs/slint/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/helper_crates/const-field-offset/src/lib.rs` & `slint-1.6.0a7/helper_crates/const-field-offset/src/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/helper_crates/const-field-offset/tests/test_field_offset.rs` & `slint-1.6.0a7/helper_crates/const-field-offset/tests/test_field_offset.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/python/Cargo.toml` & `slint-1.6.0a7/api/python/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/python/README.md` & `slint-1.6.0a7/api/python/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,15 @@
 ```
 
 1. Create a file called `main.py`:
 
 ```python
 import slint
 
+# slint.loader will look in `sys.path` for `appwindow.slint`.
 class App(slint.loader.appwindow.AppWindow):
     @slint.callback
     def request_increase_value(self):
         self.counter = self.counter + 1
 
 app = App()
 app.run()
```

### Comparing `slint-1.6.0a6/api/python/brush.rs` & `slint-1.6.0a7/api/python/brush.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/python/errors.rs` & `slint-1.6.0a7/api/python/errors.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/python/image.rs` & `slint-1.6.0a7/api/python/image.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/python/interpreter.rs` & `slint-1.6.0a7/api/python/interpreter.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/python/lib.rs` & `slint-1.6.0a7/api/python/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/python/models.rs` & `slint-1.6.0a7/api/python/models.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/python/slint/__init__.py` & `slint-1.6.0a7/api/python/slint/__init__.py`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/python/slint/models.py` & `slint-1.6.0a7/api/python/slint/models.py`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/python/tests/test_brush.py` & `slint-1.6.0a7/api/python/tests/test_brush.py`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/python/tests/test_callback_decorators.py` & `slint-1.6.0a7/api/python/tests/test_callback_decorators.py`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/python/tests/test_compiler.py` & `slint-1.6.0a7/api/python/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/python/tests/test_gc.py` & `slint-1.6.0a7/api/python/tests/test_gc.py`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/python/tests/test_instance.py` & `slint-1.6.0a7/api/python/tests/test_instance.py`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/python/tests/test_load_file.py` & `slint-1.6.0a7/api/python/tests/test_load_file.py`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/python/tests/test_load_file.slint` & `slint-1.6.0a7/api/python/tests/test_load_file.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/python/tests/test_loader.py` & `slint-1.6.0a7/api/python/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/python/tests/test_models.py` & `slint-1.6.0a7/api/python/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/python/tests/test_timers.py` & `slint-1.6.0a7/api/python/tests/test_timers.py`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/api/python/timer.rs` & `slint-1.6.0a7/api/python/timer.rs`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         match value {
             PyTimerMode::SingleShot => i_slint_core::timers::TimerMode::SingleShot,
             PyTimerMode::Repeated => i_slint_core::timers::TimerMode::Repeated,
         }
     }
 }
 
-#[pyclass(name = "Timer")]
+#[pyclass(name = "Timer", unsendable)]
 pub struct PyTimer {
     timer: i_slint_core::timers::Timer,
 }
 
 #[pymethods]
 impl PyTimer {
     #[new]
```

### Comparing `slint-1.6.0a6/api/python/value.rs` & `slint-1.6.0a7/api/python/value.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/Cargo.lock` & `slint-1.6.0a7/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93d80d7aa92a9334120580e9fe2028670f48f2b1a30cdf8bfd3d038c2f430345"
 dependencies = [
  "accesskit",
  "accesskit_macos",
  "accesskit_unix",
  "accesskit_windows",
- "raw-window-handle 0.6.0",
+ "raw-window-handle 0.6.1",
  "winit",
 ]
 
 [[package]]
 name = "addr2line"
 version = "0.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -219,55 +219,56 @@
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "anstream"
-version = "0.6.13"
+version = "0.6.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d96bd03f33fe50a863e394ee9718a706f988b9079b20c3784fb726e7678b62fb"
+checksum = "418c75fa768af9c03be99d17643f93f79bbba589895012a80e3452a19ddda15b"
 dependencies = [
  "anstyle",
  "anstyle-parse",
  "anstyle-query",
  "anstyle-wincon",
  "colorchoice",
+ "is_terminal_polyfill",
  "utf8parse",
 ]
 
 [[package]]
 name = "anstyle"
-version = "1.0.6"
+version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8901269c6307e8d93993578286ac0edf7f195079ffff5ebdeea6a59ffb7e36bc"
+checksum = "038dfcf04a5feb68e9c60b21c9625a54c2c0616e79b72b0fd87075a056ae1d1b"
 
 [[package]]
 name = "anstyle-parse"
-version = "0.2.3"
+version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c75ac65da39e5fe5ab759307499ddad880d724eed2f6ce5b5e8a26f4f387928c"
+checksum = "c03a11a9034d92058ceb6ee011ce58af4a9bf61491aa7e1e59ecd24bd40d22d4"
 dependencies = [
  "utf8parse",
 ]
 
 [[package]]
 name = "anstyle-query"
-version = "1.0.2"
+version = "1.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e28923312444cdd728e4738b3f9c9cac739500909bb3d3c94b43551b16517648"
+checksum = "a64c907d4e79225ac72e2a354c9ce84d50ebb4586dee56c82b3ee73004f537f5"
 dependencies = [
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "anstyle-wincon"
-version = "3.0.2"
+version = "3.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1cd54b81ec8d6180e24654d0b371ad22fc3dd083b6ff8ba325b72e00c87660a7"
+checksum = "61a38449feb7068f52bb06c12759005cf459ee52bb4adc1d5a7c4322d716fb19"
 dependencies = [
  "anstyle",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "anyhow"
@@ -316,28 +317,28 @@
 name = "async-channel"
 version = "2.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "136d4d23bcc79e27423727b36823d86233aad06dfea531837b038394d11e9928"
 dependencies = [
  "concurrent-queue",
  "event-listener 5.3.0",
- "event-listener-strategy 0.5.1",
+ "event-listener-strategy 0.5.2",
  "futures-core",
  "pin-project-lite",
 ]
 
 [[package]]
 name = "async-executor"
 version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b10202063978b3351199d68f8b22c4e47e4b1b822f8d43fd862d5ea8c006b29a"
 dependencies = [
  "async-task",
  "concurrent-queue",
- "fastrand 2.0.2",
+ "fastrand 2.1.0",
  "futures-lite 2.3.0",
  "slab",
 ]
 
 [[package]]
 name = "async-fs"
 version = "1.6.0"
@@ -348,17 +349,17 @@
  "autocfg",
  "blocking",
  "futures-lite 1.13.0",
 ]
 
 [[package]]
 name = "async-fs"
-version = "2.1.1"
+version = "2.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bc19683171f287921f2405677dd2ed2549c3b3bda697a563ebc3a121ace2aba1"
+checksum = "ebcd09b382f40fcd159c2d695175b2ae620ffa5f3bd6f664131efff4e8b9e04a"
 dependencies = [
  "async-lock 3.3.0",
  "blocking",
  "futures-lite 2.3.0",
 ]
 
 [[package]]
@@ -389,16 +390,16 @@
 dependencies = [
  "async-lock 3.3.0",
  "cfg-if",
  "concurrent-queue",
  "futures-io",
  "futures-lite 2.3.0",
  "parking",
- "polling 3.6.0",
- "rustix 0.38.32",
+ "polling 3.7.0",
+ "rustix 0.38.34",
  "slab",
  "tracing",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "async-lock"
@@ -440,72 +441,72 @@
  "async-io 1.13.0",
  "async-lock 2.8.0",
  "async-signal",
  "blocking",
  "cfg-if",
  "event-listener 3.1.0",
  "futures-lite 1.13.0",
- "rustix 0.38.32",
+ "rustix 0.38.34",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "async-process"
-version = "2.2.1"
+version = "2.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cad07b3443bfa10dcddf86a452ec48949e8e7fedf7392d82de3969fda99e90ed"
+checksum = "a53fc6301894e04a92cb2584fedde80cb25ba8e02d9dc39d4a87d036e22f397d"
 dependencies = [
  "async-channel",
  "async-io 2.3.2",
  "async-lock 3.3.0",
  "async-signal",
  "async-task",
  "blocking",
  "cfg-if",
  "event-listener 5.3.0",
  "futures-lite 2.3.0",
- "rustix 0.38.32",
+ "rustix 0.38.34",
  "tracing",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "async-recursion"
-version = "1.1.0"
+version = "1.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "30c5ef0ede93efbf733c1a727f3b6b5a1060bbedd5600183e66f6e4be4af0ec5"
+checksum = "3b43422f69d8ff38f95f1b2bb76517c91589a924d1559a0e935d7c8ce0274c11"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.60",
 ]
 
 [[package]]
 name = "async-signal"
-version = "0.2.5"
+version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e47d90f65a225c4527103a8d747001fc56e375203592b25ad103e1ca13124c5"
+checksum = "afe66191c335039c7bb78f99dc7520b0cbb166b3a1cb33a03f53d8a1c6f2afda"
 dependencies = [
  "async-io 2.3.2",
- "async-lock 2.8.0",
+ "async-lock 3.3.0",
  "atomic-waker",
  "cfg-if",
  "futures-core",
  "futures-io",
- "rustix 0.38.32",
+ "rustix 0.38.34",
  "signal-hook-registry",
  "slab",
- "windows-sys 0.48.0",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "async-task"
-version = "4.7.0"
+version = "4.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fbb36e985947064623dbd357f727af08ffd077f93d696782f3c56365fa2e2799"
+checksum = "8b75356056920673b02621b35afd0f7dda9306d03c79a30f5c56c44cf256e3de"
 
 [[package]]
 name = "async-trait"
 version = "0.1.80"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c6fa2087f2753a7da8cc1c0dbfcf89579dd57458e36769de5ac750b4671737ca"
 dependencies = [
@@ -640,14 +641,20 @@
 [[package]]
 name = "base64"
 version = "0.21.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9d297deb1925b89f2ccc13d7635fa0714f12c87adce1c75356b39ca9b7178567"
 
 [[package]]
+name = "base64"
+version = "0.22.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "72b3254f16251a8381aa12e40e3c4d2f0199f8c6508fbecb9d91f575e0fbb8c6"
+
+[[package]]
 name = "basic-toml"
 version = "0.1.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "823388e228f614e9558c6804262db37960ec8821856535f5c3f59913140558f8"
 dependencies = [
  "serde",
 ]
@@ -767,26 +774,24 @@
 dependencies = [
  "block-sys",
  "objc2 0.5.1",
 ]
 
 [[package]]
 name = "blocking"
-version = "1.5.1"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6a37913e8dc4ddcc604f0c6d3bf2887c995153af3611de9e23c352b44c1b9118"
+checksum = "495f7104e962b7356f0aeb34247aca1fe7d2e783b346582db7f2904cb5717e88"
 dependencies = [
  "async-channel",
  "async-lock 3.3.0",
  "async-task",
- "fastrand 2.0.2",
  "futures-io",
  "futures-lite 2.3.0",
  "piper",
- "tracing",
 ]
 
 [[package]]
 name = "bondrewd"
 version = "0.1.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6d1660fac8d3acced44dac64453fafedf5aab2de196b932c727e63e4ae42d1cc"
@@ -859,28 +864,28 @@
 name = "calloop"
 version = "0.12.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fba7adb4dd5aa98e5553510223000e7148f621165ec5f9acd7113f6ca4995298"
 dependencies = [
  "bitflags 2.5.0",
  "log",
- "polling 3.6.0",
- "rustix 0.38.32",
+ "polling 3.7.0",
+ "rustix 0.38.34",
  "slab",
  "thiserror",
 ]
 
 [[package]]
 name = "calloop-wayland-source"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0f0ea9b9476c7fad82841a8dbb380e2eae480c21910feba80725b46931ed8f02"
 dependencies = [
  "calloop",
- "rustix 0.38.32",
+ "rustix 0.38.34",
  "wayland-backend",
  "wayland-client",
 ]
 
 [[package]]
 name = "carousel"
 version = "1.6.0"
@@ -912,20 +917,21 @@
  "syn 1.0.109",
  "tempfile",
  "toml 0.5.11",
 ]
 
 [[package]]
 name = "cc"
-version = "1.0.94"
+version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "17f6e324229dc011159fcc089755d1e2e216a90d43a7dea6853ca740b84f35e7"
+checksum = "065a29261d53ba54260972629f9ca6bffa69bac13cd1fed61420f7fa68b9f8bd"
 dependencies = [
  "jobserver",
  "libc",
+ "once_cell",
 ]
 
 [[package]]
 name = "cesu8"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6d43a04d8753f35258c91f8ec639f792891f748a1edbd759cf1dcea3382ad83c"
@@ -1050,17 +1056,17 @@
 dependencies = [
  "lazy-bytes-cast",
  "winapi",
 ]
 
 [[package]]
 name = "clru"
-version = "0.6.1"
+version = "0.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b8191fa7302e03607ff0e237d4246cc043ff5b3cb9409d995172ba3bea16b807"
+checksum = "cbd0f76e066e64fdc5631e3bb46381254deab9ef1158292f27c8c57e3bf3fe59"
 
 [[package]]
 name = "cocoa"
 version = "0.25.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f6140449f97a6e97f9511815c5632d84c8aacf8ac271ad77c559218161a1373c"
 dependencies = [
@@ -1108,38 +1114,44 @@
 name = "color_quant"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3d7b894f5411737b7867f4827955924d7c254fc9f4d91a6aad6b097804b1018b"
 
 [[package]]
 name = "colorchoice"
-version = "1.0.0"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "acbf1af155f9b9ef647e42cdc158db4b64a1b61f743629225fde6f3e0be2a7c7"
+checksum = "0b6a852b24ab71dffc585bcb46eaf7959d175cb865a7152e35b348d1b2960422"
 
 [[package]]
 name = "combine"
 version = "4.6.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ba5a308b75df32fe02788e748662718f03fde005016435c444eea572398219fd"
 dependencies = [
  "bytes",
  "memchr",
 ]
 
 [[package]]
 name = "concurrent-queue"
-version = "2.4.0"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d16048cd947b08fa32c24458a22f5dc5e835264f689f4f5653210c69fd107363"
+checksum = "4ca0197aee26d1ae37445ee532fefce43251d24cc7c166799f4d46817f1d3973"
 dependencies = [
  "crossbeam-utils",
 ]
 
 [[package]]
+name = "condtype"
+version = "1.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "baf0a07a401f374238ab8e2f11a104d2851bf9ce711ec69804834de8af45c7af"
+
+[[package]]
 name = "console_error_panic_hook"
 version = "0.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a06aeb73f470f66dcdbf7223caeebb85984942f22f1adb2a088cf9668146bbbc"
 dependencies = [
  "cfg-if",
  "wasm-bindgen",
@@ -1449,17 +1461,17 @@
 checksum = "53fe5e26ff1b7aef8bca9c6080520cfb8d9333c7568e1829cef191a9723e5504"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "crc-any"
-version = "2.4.4"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c01a5e1f881f6fb6099a7bdf949e946719fd4f1fefa56264890574febf0eb6d0"
+checksum = "a62ec9ff5f7965e4d7280bd5482acd20aadb50d632cf6c1d74493856b011fa73"
 dependencies = [
  "debug-helper",
 ]
 
 [[package]]
 name = "crc32fast"
 version = "1.4.0"
@@ -1766,17 +1778,42 @@
  "byte-slice-cast",
  "display-interface",
  "embedded-hal",
 ]
 
 [[package]]
 name = "dissimilar"
-version = "1.0.7"
+version = "1.0.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "440d59c0c6d96354061909b4769b2ca03868dbaee203e7b779d9021ebbde3058"
+
+[[package]]
+name = "divan"
+version = "0.1.14"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a0d567df2c9c2870a43f3f2bd65aaeb18dbce1c18f217c3e564b4fbaeb3ee56c"
+dependencies = [
+ "cfg-if",
+ "clap",
+ "condtype",
+ "divan-macros",
+ "libc",
+ "regex-lite",
+]
+
+[[package]]
+name = "divan-macros"
+version = "0.1.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "86e3bdc80eee6e16b2b6b0f87fbc98c04bee3455e35174c0de1a125d0688c632"
+checksum = "27540baf49be0d484d8f0130d7d8da3011c32a44d4fc873368154f1510e574a2"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.60",
+]
 
 [[package]]
 name = "dlib"
 version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "330c60081dcc4c72131f8eb70510f1ac07223e5d4163db481a04a0befcffa412"
 dependencies = [
@@ -1826,15 +1863,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a0f8a69e60d75ae7dab4ef26a59ca99f2a89d4c142089b537775ae0c198bdcde"
 dependencies = [
  "bitflags 2.5.0",
  "bytemuck",
  "drm-ffi 0.7.1",
  "drm-fourcc",
- "rustix 0.38.32",
+ "rustix 0.38.34",
 ]
 
 [[package]]
 name = "drm-ffi"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1352481b7b90e27a8a1bf8ef6b33cf18b98dba7c410e75c24bb3eef2f0d8d525"
@@ -1846,15 +1883,15 @@
 [[package]]
 name = "drm-ffi"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "41334f8405792483e32ad05fbb9c5680ff4e84491883d2947a4757dc54cb2ac6"
 dependencies = [
  "drm-sys 0.6.1",
- "rustix 0.38.32",
+ "rustix 0.38.34",
 ]
 
 [[package]]
 name = "drm-fourcc"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0aafbcdb8afc29c1a7ee5fbe53b5d62f4565b35a042a662ca9fecd0b54dae6f4"
@@ -2280,17 +2317,17 @@
 dependencies = [
  "event-listener 4.0.3",
  "pin-project-lite",
 ]
 
 [[package]]
 name = "event-listener-strategy"
-version = "0.5.1"
+version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "332f51cb23d20b0de8458b86580878211da09bcd4503cb579c225b3d124cabb3"
+checksum = "0f214dc438f977e6d4e3500aaa277f5ad94ca83fbbd9b1a15713ce2344ccc5a1"
 dependencies = [
  "event-listener 5.3.0",
  "pin-project-lite",
 ]
 
 [[package]]
 name = "exr"
@@ -2315,17 +2352,17 @@
 checksum = "e51093e27b0797c359783294ca4f0a911c270184cb10f85783b118614a1501be"
 dependencies = [
  "instant",
 ]
 
 [[package]]
 name = "fastrand"
-version = "2.0.2"
+version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "658bd65b1cf4c852a3cc96f18a8ce7b5640f6b703f905c7d74532294c2a63984"
+checksum = "9fc0510504f03c51ada170672ac806f1f105a88aa97a5281117e1ddc3368e51a"
 
 [[package]]
 name = "fdeflate"
 version = "0.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4f9bfee30e4dedf0ab8b422f03af778d9612b63f502710fc500a334ebe2de645"
 dependencies = [
@@ -2342,15 +2379,15 @@
  "fnv",
  "glow",
  "image",
  "imgref",
  "log",
  "lru",
  "rgb",
- "rustybuzz 0.13.0",
+ "rustybuzz",
  "slotmap",
  "unicode-bidi",
  "unicode-segmentation",
  "wasm-bindgen",
  "web-sys",
 ]
 
@@ -2430,17 +2467,17 @@
  "libc",
  "redox_syscall 0.4.1",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "flate2"
-version = "1.0.28"
+version = "1.0.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "46303f565772937ffe1d394a4fac6f411c6013172fadde9dcdb1e147a086940e"
+checksum = "5f54427cfd1c7829e2a139fcefea601bf088ebca651d2bf53ebc600eac295dae"
 dependencies = [
  "crc32fast",
  "miniz_oxide",
 ]
 
 [[package]]
 name = "float-cmp"
@@ -2531,15 +2568,15 @@
 
 [[package]]
 name = "fontdue"
 version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9099a2f86b8e674b75d03ff154b3fe4c5208ed249ced8d69cc313a9fa40bb488"
 dependencies = [
- "hashbrown 0.14.3",
+ "hashbrown 0.14.5",
  "ttf-parser 0.20.0",
 ]
 
 [[package]]
 name = "foreign-types"
 version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2588,27 +2625,27 @@
 checksum = "e13624c2627564efccf4934284bdd98cbaa14e79b0b5a141218e507b3a823456"
 dependencies = [
  "percent-encoding",
 ]
 
 [[package]]
 name = "freetype"
-version = "0.7.1"
+version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "efc8599a3078adf8edeb86c71e9f8fa7d88af5ca31e806a867756081f90f5d83"
+checksum = "5a440748e063798e4893ceb877151e84acef9bea9a8c6800645cf3f1b3a7806e"
 dependencies = [
  "freetype-sys",
  "libc",
 ]
 
 [[package]]
 name = "freetype-sys"
-version = "0.19.0"
+version = "0.20.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "66ee28c39a43d89fbed8b4798fb4ba56722cfd2b5af81f9326c27614ba88ecd5"
+checksum = "0e7edc5b9669349acfda99533e9e0bcf26a51862ab43b08ee7745c55d28eb134"
 dependencies = [
  "cc",
  "libc",
  "pkg-config",
 ]
 
 [[package]]
@@ -2733,15 +2770,15 @@
 
 [[package]]
 name = "futures-lite"
 version = "2.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "52527eb5074e35e9339c6b4e8d12600c7128b68fb25dcb9fa9dec18f7c25f3a5"
 dependencies = [
- "fastrand 2.0.2",
+ "fastrand 2.1.0",
  "futures-core",
  "futures-io",
  "parking",
  "pin-project-lite",
 ]
 
 [[package]]
@@ -3276,17 +3313,17 @@
 name = "hashbrown"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
 
 [[package]]
 name = "hashbrown"
-version = "0.14.3"
+version = "0.14.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "290f1a1d9242c78d09ce40a5e87e7554ee637af1351968159f4952f028f75604"
+checksum = "e5274423e17b7c9fc20b6e7e208532f9b19825d82dfd615708b70edd83df41f1"
 dependencies = [
  "ahash",
  "allocator-api2",
 ]
 
 [[package]]
 name = "heapless"
@@ -3387,15 +3424,15 @@
  "h2",
  "http",
  "http-body",
  "httparse",
  "httpdate",
  "itoa",
  "pin-project-lite",
- "socket2 0.5.6",
+ "socket2 0.5.7",
  "tokio",
  "tower-service",
  "tracing",
  "want",
 ]
 
 [[package]]
@@ -3476,14 +3513,16 @@
 ]
 
 [[package]]
 name = "i-slint-backend-testing"
 version = "1.6.0"
 dependencies = [
  "i-slint-core",
+ "i-slint-core-macros",
+ "slint",
  "vtable",
 ]
 
 [[package]]
 name = "i-slint-backend-winit"
 version = "1.6.0"
 dependencies = [
@@ -3504,15 +3543,15 @@
  "i-slint-renderer-femtovg",
  "i-slint-renderer-skia",
  "imgref",
  "lyon_path",
  "once_cell",
  "pin-weak",
  "raw-window-handle 0.5.2",
- "raw-window-handle 0.6.0",
+ "raw-window-handle 0.6.1",
  "rgb",
  "scoped-tls-hkt",
  "scopeguard",
  "slint",
  "softbuffer",
  "wasm-bindgen",
  "web-sys",
@@ -3586,18 +3625,18 @@
  "lyon_geom",
  "lyon_path",
  "num-traits",
  "once_cell",
  "pin-project",
  "pin-weak",
  "portable-atomic",
- "raw-window-handle 0.6.0",
+ "raw-window-handle 0.6.1",
  "resvg",
  "rgb",
- "rustybuzz 0.13.0",
+ "rustybuzz",
  "scoped-tls-hkt",
  "scopeguard",
  "serde",
  "serde_json",
  "slab",
  "slint",
  "static_assertions",
@@ -3805,15 +3844,15 @@
 [[package]]
 name = "indexmap"
 version = "2.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "168fb715dda47215e360912c096649d23d58bf392ac62f73919e831745e40f26"
 dependencies = [
  "equivalent",
- "hashbrown 0.14.3",
+ "hashbrown 0.14.5",
 ]
 
 [[package]]
 name = "indoc"
 version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
@@ -3890,14 +3929,20 @@
 [[package]]
 name = "ipnet"
 version = "2.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f518f335dce6725a761382244631d86cf0ccb2863413590b31338feb467f9c3"
 
 [[package]]
+name = "is_terminal_polyfill"
+version = "1.70.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f8478577c03552c21db0e2724ffb8986a5ce7af88107e6be5d2ee6e158c12800"
+
+[[package]]
 name = "itertools"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
@@ -3949,17 +3994,17 @@
 name = "jni-sys"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8eaf4bc02d17cbdd7ff4c7438cafcdf7fb9a4613313ad11b4f8fefe7d3fa0130"
 
 [[package]]
 name = "jobserver"
-version = "0.1.30"
+version = "0.1.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "685a7d121ee3f65ae4fddd72b25a04bb36b6af81bc0828f7d5434c0fe60fa3a2"
+checksum = "d2b099aaa34a9751c5bf0878add70444e1ed2dd73f347be99003d4577277de6e"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "jpeg-decoder"
 version = "0.3.1"
@@ -4002,26 +4047,17 @@
 dependencies = [
  "bitflags 1.3.2",
  "libc",
 ]
 
 [[package]]
 name = "kurbo"
-version = "0.9.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd85a5776cd9500c2e2059c8c76c3b01528566b7fcbaf8098b55a33fc298849b"
-dependencies = [
- "arrayvec",
-]
-
-[[package]]
-name = "kurbo"
-version = "0.10.4"
+version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1618d4ebd923e97d67e7cd363d80aef35fe961005cbbbb3d2dad8bdd1bc63440"
+checksum = "6e5aa9f0f96a938266bdb12928a67169e8d22c6a786fda8ed984b85e6ba93c3c"
 dependencies = [
  "arrayvec",
  "smallvec",
 ]
 
 [[package]]
 name = "lazy-bytes-cast"
@@ -4045,17 +4081,17 @@
 name = "lebe"
 version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "03087c2bad5e1034e8cace5926dec053fb3790248370865f5117a7d0213354c8"
 
 [[package]]
 name = "libc"
-version = "0.2.153"
+version = "0.2.154"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
+checksum = "ae743338b92ff9146ce83992f766a31066a91a8c84a45e0e9f21e7cf6de6d346"
 
 [[package]]
 name = "libloading"
 version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b67380fd3b2fbe7527a606e18729d21c6f3951633d0500574c4dc22d2d638b9f"
 dependencies = [
@@ -4195,17 +4231,17 @@
  "objc-foundation",
  "regex",
  "winapi",
 ]
 
 [[package]]
 name = "lock_api"
-version = "0.4.11"
+version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
+checksum = "07af8b9cdd281b7915f413fa73f29ebd5d55d0d3f0155584dade1ff18cea1b17"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
@@ -4252,19 +4288,20 @@
 dependencies = [
  "lyon_path",
  "num-traits",
 ]
 
 [[package]]
 name = "lyon_extra"
-version = "1.0.1"
+version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b9ce2ae38f2480094ec1f0d5df51a75581fa84f0e8f32a0edb1d264630c99f3b"
+checksum = "8c4a243ce61e7e5f3ae6c72a88d8fb081b6c69f13500c15e99cfd1159a833b20"
 dependencies = [
  "lyon_path",
+ "thiserror",
 ]
 
 [[package]]
 name = "lyon_geom"
 version = "1.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "edecfb8d234a2b0be031ab02ebcdd9f3b9ee418fb35e265f7a540a48d197bff9"
@@ -4421,28 +4458,34 @@
 name = "mime"
 version = "0.3.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6877bb514081ee2a7ff5ef9de3281f14a4dd4bceac4c09388074a6b5df8a139a"
 
 [[package]]
 name = "minijinja"
-version = "1.0.20"
+version = "1.0.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb5c5e3d2b4c0a6832bd3d571f7c19a7c1c1f05f11a6e85ae1a29f76be5f9455"
+checksum = "55e877d961d4f96ce13615862322df7c0b6d169d40cab71a7ef3f9b9e594451e"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "minimal-lexical"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "68354c5c6bd36d73ff3feceb05efa59b6acb7626617f4962be322a825e61f79a"
 
 [[package]]
+name = "minipng"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "44aaf824f3dbcc8a4ab8fd66964fed5200a632d5794775a2426e77e3833776a8"
+
+[[package]]
 name = "miniz_oxide"
 version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9d811f3e15f28568be3407c8e7fdb6514c1cda3cb30683f15b6a1a1dc4ea14a7"
 dependencies = [
  "adler",
  "simd-adler32",
@@ -4583,15 +4626,15 @@
 dependencies = [
  "bitflags 2.5.0",
  "jni-sys",
  "log",
  "ndk-sys",
  "num_enum 0.7.2",
  "raw-window-handle 0.5.2",
- "raw-window-handle 0.6.0",
+ "raw-window-handle 0.6.1",
  "thiserror",
 ]
 
 [[package]]
 name = "ndk-context"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -5026,33 +5069,33 @@
 name = "parking"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bb813b8af86854136c6922af0598d719255ecb2179515e6e7730d468f05c9cae"
 
 [[package]]
 name = "parking_lot"
-version = "0.12.1"
+version = "0.12.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
+checksum = "7e4af0ca4f6caed20e900d564c242b8e5d4903fdacf31d3daf527b66fe6f42fb"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.9"
+version = "0.9.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
+checksum = "1e401f977ab385c9e4e3ab30627d6f26d00e2c73eef317493c4ec6d468726cf8"
 dependencies = [
  "cfg-if",
  "libc",
- "redox_syscall 0.4.1",
+ "redox_syscall 0.5.1",
  "smallvec",
- "windows-targets 0.48.5",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "paste"
 version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "de3145af08024dea9fa9914f381a17b8fc6034dfb00f3a84013f7ff43f29ed4c"
@@ -5146,15 +5189,15 @@
 [[package]]
 name = "piper"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "668d31b1c4eba19242f2088b2bf3316b82ca31082a8335764db4e083db7485d4"
 dependencies = [
  "atomic-waker",
- "fastrand 2.0.2",
+ "fastrand 2.1.0",
  "futures-io",
 ]
 
 [[package]]
 name = "pkg-config"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -5237,23 +5280,23 @@
  "log",
  "pin-project-lite",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "polling"
-version = "3.6.0"
+version = "3.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e0c976a60b2d7e99d6f229e414670a9b85d13ac305cc6d1e9c134de58c5aaaf6"
+checksum = "645493cf344456ef24219d02a768cf1fb92ddf8c92161679ae3d91b91a637be3"
 dependencies = [
  "cfg-if",
  "concurrent-queue",
  "hermit-abi",
  "pin-project-lite",
- "rustix 0.38.32",
+ "rustix 0.38.34",
  "tracing",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "portable-atomic"
 version = "1.6.0"
@@ -5297,14 +5340,15 @@
  "web-sys",
 ]
 
 [[package]]
 name = "printerdemo_mcu"
 version = "1.6.0"
 dependencies = [
+ "divan",
  "mcu-board-support",
  "slint",
  "slint-build",
 ]
 
 [[package]]
 name = "printerdemo_old"
@@ -5538,17 +5582,17 @@
 name = "raw-window-handle"
 version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f2ff9a1f06a88b01621b7ae906ef0211290d1c8a168a15542486a8f61c0833b9"
 
 [[package]]
 name = "raw-window-handle"
-version = "0.6.0"
+version = "0.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "42a9830a0e1b9fb145ebb365b8bc4ccd75f290f98c0247deafbbe2c75cefb544"
+checksum = "8cc3bcbdb1ddfc11e700e62968e6b4cc9c75bb466464ad28fb61c5b2c964418b"
 
 [[package]]
 name = "rayon"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b418a60154510ca1a002a752ca9714984e21e4241e804d32555251faf8b78ffa"
 dependencies = [
@@ -5581,14 +5625,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags 1.3.2",
 ]
 
 [[package]]
+name = "redox_syscall"
+version = "0.5.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
+dependencies = [
+ "bitflags 2.5.0",
+]
+
+[[package]]
 name = "redox_users"
 version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bd283d9651eeda4b2a83a43c1c91b266c40fd76ecd39a50a8c630ae69dc72891"
 dependencies = [
  "getrandom",
  "libredox 0.1.3",
@@ -5615,26 +5668,32 @@
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
+name = "regex-lite"
+version = "0.1.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "30b661b2f27137bdbc16f00eda72866a92bb28af1753ffbd56744fb6e2e9cd8e"
+
+[[package]]
 name = "regex-syntax"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "reqwest"
 version = "0.11.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dd67538700a17451e7cba03ac727fb961abb7607553461627b97de0b89cf4a62"
 dependencies = [
- "base64",
+ "base64 0.21.7",
  "bytes",
  "encoding_rs",
  "futures-core",
  "futures-util",
  "h2",
  "http",
  "http-body",
@@ -5664,17 +5723,17 @@
  "wasm-streams",
  "web-sys",
  "winreg",
 ]
 
 [[package]]
 name = "resvg"
-version = "0.40.0"
+version = "0.41.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "024e40e1ba7313fc315b1720298988c0cd6f8bfe3754b52838aafecebd11355a"
+checksum = "c2327ced609dadeed3e9702fec3e6b2ddd208758a9268d13e06566c6101ba533"
 dependencies = [
  "log",
  "pico-args",
  "rgb",
  "svgtypes",
  "tiny-skia",
  "usvg",
@@ -5716,15 +5775,15 @@
 [[package]]
 name = "rowan"
 version = "0.15.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "32a58fa8a7ccff2aec4f39cc45bf5f985cec7125ab271cf681c279fd00192b49"
 dependencies = [
  "countme",
- "hashbrown 0.14.3",
+ "hashbrown 0.14.5",
  "memoffset 0.9.1",
  "rustc-hash",
  "text-size",
 ]
 
 [[package]]
 name = "roxmltree"
@@ -5844,30 +5903,30 @@
  "libc",
  "linux-raw-sys 0.3.8",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.38.32"
+version = "0.38.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "65e04861e65f21776e67888bfbea442b3642beaa0138fdb1dd7a84a52dffdb89"
+checksum = "70dc5ec042f7a43c4a73241207cecc9873a06d45debb38b329f8541d85c2730f"
 dependencies = [
  "bitflags 2.5.0",
  "errno",
  "libc",
  "linux-raw-sys 0.4.13",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "rustls"
-version = "0.22.3"
+version = "0.22.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "99008d7ad0bbbea527ec27bddbc0e432c5b87d8175178cee68d2eec9c4a1813c"
+checksum = "bf4ef73721ac7bcd79b2b315da7779d8fc09718c6b3d2d1b2d94850eb8c18432"
 dependencies = [
  "log",
  "ring",
  "rustls-pki-types",
  "rustls-webpki",
  "subtle",
  "zeroize",
@@ -5875,68 +5934,52 @@
 
 [[package]]
 name = "rustls-pemfile"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1c74cae0a4cf6ccbbf5f359f08efdf8ee7e1dc532573bf0db71968cb56b1448c"
 dependencies = [
- "base64",
+ "base64 0.21.7",
 ]
 
 [[package]]
 name = "rustls-pki-types"
-version = "1.4.1"
+version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ecd36cc4259e3e4514335c4a138c6b43171a8d61d8f5c9348f9fc7529416f247"
+checksum = "beb461507cee2c2ff151784c52762cf4d9ff6a61f3e80968600ed24fa837fa54"
 
 [[package]]
 name = "rustls-webpki"
-version = "0.102.2"
+version = "0.102.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "faaa0a62740bedb9b2ef5afa303da42764c012f743917351dc9a237ea1663610"
+checksum = "f3bce581c0dd41bce533ce695a1437fa16a7ab5ac3ccfa99fe1a620a7885eabf"
 dependencies = [
  "ring",
  "rustls-pki-types",
  "untrusted",
 ]
 
 [[package]]
 name = "rustversion"
 version = "1.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "80af6f9131f277a45a3fba6ce8e2258037bb0477a67e610d3c1fe046ab31de47"
 
 [[package]]
 name = "rustybuzz"
-version = "0.12.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f0ae5692c5beaad6a9e22830deeed7874eae8a4e3ba4076fb48e12c56856222c"
-dependencies = [
- "bitflags 2.5.0",
- "bytemuck",
- "smallvec",
- "ttf-parser 0.20.0",
- "unicode-bidi-mirroring 0.1.0",
- "unicode-ccc 0.1.2",
- "unicode-properties",
- "unicode-script",
-]
-
-[[package]]
-name = "rustybuzz"
 version = "0.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "88117946aa1bfb53c2ae0643ceac6506337f44887f8c9fbfb43587b1cc52ba49"
 dependencies = [
  "bitflags 2.5.0",
  "bytemuck",
  "smallvec",
  "ttf-parser 0.20.0",
- "unicode-bidi-mirroring 0.2.0",
- "unicode-ccc 0.2.0",
+ "unicode-bidi-mirroring",
+ "unicode-ccc",
  "unicode-properties",
  "unicode-script",
 ]
 
 [[package]]
 name = "ryu"
 version = "1.0.17"
@@ -6040,17 +6083,17 @@
 name = "send_wrapper"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cd0b0ec5f1c1ca621c432a25813d8d60c88abe6d3e08a3eb9cf37d97a0fe3d73"
 
 [[package]]
 name = "serde"
-version = "1.0.198"
+version = "1.0.200"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9846a40c979031340571da2545a4e5b7c4163bdae79b301d5f86d03979451fcc"
+checksum = "ddc6f9cc94d67c0e21aaf7eda3a010fd3af78ebf6e096aa6e2e13c79749cce4f"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde-wasm-bindgen"
 version = "0.6.5"
@@ -6060,17 +6103,17 @@
  "js-sys",
  "serde",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.198"
+version = "1.0.200"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e88edab869b01783ba905e7d0153f9fc1a6505a96e4ad3018011eedb838566d9"
+checksum = "856f046b9400cee3c8c94ed572ecdb752444c24528c035cd35882aad6f492bcb"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.60",
 ]
 
 [[package]]
@@ -6162,17 +6205,17 @@
  "libc",
  "mio",
  "signal-hook",
 ]
 
 [[package]]
 name = "signal-hook-registry"
-version = "1.4.1"
+version = "1.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d8229b473baa5980ac72ef434c4415e70c4b5e71b423043adb4ba059f89c99a1"
+checksum = "a9e9e0b4211b72e7b8b6e85c807d36c212bdb33ea8587f7569562a84df5465b1"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "simd-adler32"
 version = "0.3.7"
@@ -6186,17 +6229,17 @@
 checksum = "a11be7c62927d9427e9f40f3444d5499d868648e2edbc4e2116de69e7ec0e89d"
 dependencies = [
  "log",
 ]
 
 [[package]]
 name = "siphasher"
-version = "0.3.11"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "38b58827f4464d87d377d175e90bf58eb00fd8716ff0a62f80356b5e61555d0d"
+checksum = "56199f7ddabf13fe5074ce809e7d3f42b42ae711800501b5b16ea82ad029c39d"
 
 [[package]]
 name = "skia-bindings"
 version = "0.72.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ace7c5359ccb009880e65958eaf1e2fa68ee19ada6931300c2f1942f84abf2c3"
 dependencies = [
@@ -6253,30 +6296,30 @@
  "i-slint-backend-testing",
  "i-slint-core",
  "i-slint-renderer-femtovg",
  "log",
  "num-traits",
  "once_cell",
  "pin-weak",
- "raw-window-handle 0.6.0",
+ "raw-window-handle 0.6.1",
  "serde",
  "serde_json",
  "slint-build",
  "slint-macros",
  "vtable",
 ]
 
 [[package]]
 name = "slint-build"
 version = "1.6.0"
 dependencies = [
  "i-slint-compiler",
  "spin_on",
  "thiserror",
- "toml_edit 0.22.9",
+ "toml_edit 0.22.12",
 ]
 
 [[package]]
 name = "slint-compiler"
 version = "1.6.0"
 dependencies = [
  "clap",
@@ -6317,15 +6360,15 @@
  "i-slint-backend-testing",
  "i-slint-backend-winit",
  "i-slint-common",
  "i-slint-compiler",
  "i-slint-core",
  "lyon_path",
  "once_cell",
- "raw-window-handle 0.6.0",
+ "raw-window-handle 0.6.1",
  "spin_on",
  "thiserror",
  "vtable",
 ]
 
 [[package]]
 name = "slint-lsp"
@@ -6494,15 +6537,15 @@
  "bitflags 2.5.0",
  "calloop",
  "calloop-wayland-source",
  "cursor-icon",
  "libc",
  "log",
  "memmap2 0.9.4",
- "rustix 0.38.32",
+ "rustix 0.38.34",
  "thiserror",
  "wayland-backend",
  "wayland-client",
  "wayland-csd-frame",
  "wayland-cursor",
  "wayland-protocols",
  "wayland-protocols-wlr",
@@ -6525,19 +6568,19 @@
 name = "smol"
 version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e635339259e51ef85ac7aa29a1cd991b957047507288697a690e80ab97d07cad"
 dependencies = [
  "async-channel",
  "async-executor",
- "async-fs 2.1.1",
+ "async-fs 2.1.2",
  "async-io 2.3.2",
  "async-lock 3.3.0",
  "async-net",
- "async-process 2.2.1",
+ "async-process 2.2.2",
  "blocking",
  "futures-lite 2.3.0",
 ]
 
 [[package]]
 name = "smol_str"
 version = "0.2.1"
@@ -6555,17 +6598,17 @@
 dependencies = [
  "libc",
  "winapi",
 ]
 
 [[package]]
 name = "socket2"
-version = "0.5.6"
+version = "0.5.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "05ffd9c0a93b7543e062e759284fcf5f5e3b098501104bfbdde4d404db792871"
+checksum = "ce305eb0b4296696835b71df73eb912e0f1ffd2556a501fcede6e0c50349191c"
 dependencies = [
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "softbuffer"
@@ -6575,23 +6618,23 @@
 dependencies = [
  "as-raw-xcb-connection",
  "bytemuck",
  "cfg_aliases 0.1.1",
  "cocoa",
  "core-graphics 0.23.2",
  "drm 0.11.1",
- "fastrand 2.0.2",
+ "fastrand 2.1.0",
  "foreign-types 0.5.0",
  "js-sys",
  "log",
  "memmap2 0.9.4",
  "objc",
  "raw-window-handle 0.5.2",
  "redox_syscall 0.4.1",
- "rustix 0.38.32",
+ "rustix 0.38.34",
  "tiny-xlib",
  "wasm-bindgen",
  "wayland-backend",
  "wayland-client",
  "wayland-sys",
  "web-sys",
  "windows-sys 0.48.0",
@@ -6769,19 +6812,19 @@
 name = "subtle"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "81cdd64d312baedb58e21336b31bc043b77e01cc99033ce76ef539f78e965ebc"
 
 [[package]]
 name = "svgtypes"
-version = "0.14.0"
+version = "0.15.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "59d7618f12b51be8171a7cfdda1e7a93f79cbc57c4e7adf89a749cf671125241"
+checksum = "d97ca9a891c9c70da8139ac9d8e8ea36a210fa21bb50eccd75d4a9561c83e87f"
 dependencies = [
- "kurbo 0.10.4",
+ "kurbo",
  "siphasher",
 ]
 
 [[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -6869,16 +6912,16 @@
 [[package]]
 name = "tempfile"
 version = "3.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "85b77fafb263dd9d05cbeac119526425676db3784113aa9295c88498cbf8bff1"
 dependencies = [
  "cfg-if",
- "fastrand 2.0.2",
- "rustix 0.38.32",
+ "fastrand 2.1.0",
+ "rustix 0.38.34",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "termcolor"
 version = "1.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -6889,15 +6932,15 @@
 
 [[package]]
 name = "terminal_size"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "21bebf2b7c9e0a515f6e0f8c51dc0f8e4696391e6f1ff30379559f8365fb0df7"
 dependencies = [
- "rustix 0.38.32",
+ "rustix 0.38.34",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "test-driver-cpp"
 version = "1.6.0"
 dependencies = [
@@ -6972,26 +7015,26 @@
 name = "text-size"
 version = "1.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f18aa187839b2bdb1ad2fa35ead8c4c2976b64e4363c386d45ac0f7ee85c9233"
 
 [[package]]
 name = "thiserror"
-version = "1.0.58"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03468839009160513471e86a034bb2c5c0e4baae3b43f79ffc55c4a5427b3297"
+checksum = "f0126ad08bff79f29fc3ae6a55cc72352056dfff61e3ff8bb7129476d44b23aa"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.58"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
+checksum = "d1cd413b5d558b4c5bf3680e324a6fa5014e7b7c067a51e69dbdf47eb7148b66"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.60",
 ]
 
 [[package]]
@@ -7069,14 +7112,15 @@
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "todo"
 version = "1.6.0"
 dependencies = [
  "console_error_panic_hook",
+ "i-slint-backend-testing",
  "serde",
  "serde_json",
  "slint",
  "slint-build",
  "wasm-bindgen",
 ]
 
@@ -7090,15 +7134,15 @@
  "bytes",
  "libc",
  "mio",
  "num_cpus",
  "parking_lot",
  "pin-project-lite",
  "signal-hook-registry",
- "socket2 0.5.6",
+ "socket2 0.5.7",
  "tokio-macros",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "tokio-macros"
 version = "2.2.0"
@@ -7148,15 +7192,15 @@
 version = "0.8.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e9dd1545e8208b4a5af1aa9bbd0b4cf7e9ea08fabc5d0a5c67fcaafa17433aa3"
 dependencies = [
  "serde",
  "serde_spanned",
  "toml_datetime",
- "toml_edit 0.22.9",
+ "toml_edit 0.22.12",
 ]
 
 [[package]]
 name = "toml_datetime"
 version = "0.6.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3550f4e9685620ac18a50ed434eb3aec30db8ba93b0287467bca5826ea25baf1"
@@ -7195,23 +7239,23 @@
  "indexmap 2.2.6",
  "toml_datetime",
  "winnow 0.5.40",
 ]
 
 [[package]]
 name = "toml_edit"
-version = "0.22.9"
+version = "0.22.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e40bb779c5187258fd7aad0eb68cb8706a0a81fa712fbea808ab43c4b8374c4"
+checksum = "d3328d4f68a705b2a4498da1d580585d39a6510f98318a2cec3018a7ec61ddef"
 dependencies = [
  "indexmap 2.2.6",
  "serde",
  "serde_spanned",
  "toml_datetime",
- "winnow 0.6.6",
+ "winnow 0.6.7",
 ]
 
 [[package]]
 name = "tower-service"
 version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b6bc1c9ce2b5135ac7f93c72918fc37feb872bdc6a5533a8b85eb4b86bfdae52"
@@ -7325,14 +7369,16 @@
  "uefi-macros",
 ]
 
 [[package]]
 name = "uefi-demo"
 version = "1.6.0"
 dependencies = [
+ "log",
+ "minipng",
  "slint",
  "slint-build",
  "uefi",
  "uefi-services",
 ]
 
 [[package]]
@@ -7361,32 +7407,20 @@
 name = "unicode-bidi"
 version = "0.3.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08f95100a766bf4f8f28f90d77e0a5461bbdb219042e7679bebe79004fed8d75"
 
 [[package]]
 name = "unicode-bidi-mirroring"
-version = "0.1.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "56d12260fb92d52f9008be7e4bca09f584780eb2266dc8fecc6a192bec561694"
-
-[[package]]
-name = "unicode-bidi-mirroring"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "23cb788ffebc92c5948d0e997106233eeb1d8b9512f93f41651f52b6c5f5af86"
 
 [[package]]
 name = "unicode-ccc"
-version = "0.1.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cc2520efa644f8268dce4dcd3050eaa7fc044fca03961e9998ac7e2e92b77cf1"
-
-[[package]]
-name = "unicode-ccc"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1df77b101bcc4ea3d78dafc5ad7e4f58ceffe0b2b16bf446aeb50b6cb4157656"
 
 [[package]]
 name = "unicode-ident"
 version = "1.0.12"
@@ -7448,19 +7482,19 @@
 name = "untrusted"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8ecb6da28b8a351d773b68d5825ac39017e680750f980f3a1a85cd8dd28a47c1"
 
 [[package]]
 name = "ureq"
-version = "2.9.6"
+version = "2.9.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11f214ce18d8b2cbe84ed3aa6486ed3f5b285cf8d8fbdbce9f3f767a724adc35"
+checksum = "d11a831e3c0b56e438a28308e7c810799e3c118417f342d30ecec080105395cd"
 dependencies = [
- "base64",
+ "base64 0.22.1",
  "encoding_rs",
  "flate2",
  "log",
  "once_cell",
  "rustls",
  "rustls-pki-types",
  "rustls-webpki",
@@ -7486,28 +7520,28 @@
 name = "usb-device"
 version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f6cc3adc849b5292b4075fc0d5fdcf2f24866e88e336dd27a8943090a520508"
 
 [[package]]
 name = "usvg"
-version = "0.40.0"
+version = "0.41.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c04150a94f0bfc3b2c15d4e151524d14cd06765fc6641d8b1c59a248360d4474"
+checksum = "5c704361d822337cfc00387672c7b59eaa72a1f0744f62b2a68aa228a0c6927d"
 dependencies = [
- "base64",
+ "base64 0.22.1",
  "data-url",
  "flate2",
  "fontdb",
  "imagesize",
- "kurbo 0.9.5",
+ "kurbo",
  "log",
  "pico-args",
  "roxmltree",
- "rustybuzz 0.12.1",
+ "rustybuzz",
  "simplecss",
  "siphasher",
  "strict-num",
  "svgtypes",
  "tiny-skia-path",
  "unicode-bidi",
  "unicode-script",
@@ -7740,28 +7774,28 @@
 name = "wayland-backend"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9d50fa61ce90d76474c87f5fc002828d81b32677340112b4ef08079a9d459a40"
 dependencies = [
  "cc",
  "downcast-rs",
- "rustix 0.38.32",
+ "rustix 0.38.34",
  "scoped-tls",
  "smallvec",
  "wayland-sys",
 ]
 
 [[package]]
 name = "wayland-client"
 version = "0.31.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "82fb96ee935c2cea6668ccb470fb7771f6215d1691746c2d896b447a00ad3f1f"
 dependencies = [
  "bitflags 2.5.0",
- "rustix 0.38.32",
+ "rustix 0.38.34",
  "wayland-backend",
  "wayland-scanner",
 ]
 
 [[package]]
 name = "wayland-csd-frame"
 version = "0.3.0"
@@ -7775,15 +7809,15 @@
 
 [[package]]
 name = "wayland-cursor"
 version = "0.31.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "71ce5fa868dd13d11a0d04c5e2e65726d0897be8de247c0c5a65886e283231ba"
 dependencies = [
- "rustix 0.38.32",
+ "rustix 0.38.34",
  "wayland-client",
  "xcursor",
 ]
 
 [[package]]
 name = "wayland-protocols"
 version = "0.31.2"
@@ -7908,26 +7942,26 @@
 version = "4.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87ba24419a2078cd2b0f2ede2691b6c66d8e47836da3b6db8265ebad47afbfc7"
 dependencies = [
  "either",
  "home",
  "once_cell",
- "rustix 0.38.32",
+ "rustix 0.38.34",
 ]
 
 [[package]]
 name = "which"
 version = "6.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8211e4f58a2b2805adfbefbc07bab82958fc91e3836339b1ab7ae32465dce0d7"
 dependencies = [
  "either",
  "home",
- "rustix 0.38.32",
+ "rustix 0.38.34",
  "winsafe",
 ]
 
 [[package]]
 name = "winapi"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -7941,19 +7975,19 @@
 name = "winapi-i686-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
 
 [[package]]
 name = "winapi-util"
-version = "0.1.6"
+version = "0.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f29e6f9198ba0d26b4c9f07dbe6f9ed633e1f3d5b8b414090084349e46a52596"
+checksum = "4d4cc384e1e73b93bafa6fb4f1df8c41695c8a91cf9c4c64358067d15a7b6c6b"
 dependencies = [
- "winapi",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "winapi-wsapoll"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1eafc5f679c576995526e81635d0cf9695841736712b4e892f87abbe6fed3f28"
@@ -8258,49 +8292,49 @@
  "ndk",
  "ndk-sys",
  "objc2 0.4.1",
  "once_cell",
  "orbclient",
  "percent-encoding",
  "raw-window-handle 0.5.2",
- "raw-window-handle 0.6.0",
+ "raw-window-handle 0.6.1",
  "redox_syscall 0.3.5",
- "rustix 0.38.32",
+ "rustix 0.38.34",
  "sctk-adwaita",
  "smithay-client-toolkit",
  "smol_str",
  "unicode-segmentation",
  "wasm-bindgen",
  "wasm-bindgen-futures",
  "wayland-backend",
  "wayland-client",
  "wayland-protocols",
  "wayland-protocols-plasma",
  "web-sys",
  "web-time 0.2.4",
  "windows-sys 0.48.0",
  "x11-dl",
- "x11rb 0.13.0",
+ "x11rb 0.13.1",
  "xkbcommon-dl",
 ]
 
 [[package]]
 name = "winnow"
 version = "0.5.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f593a95398737aeed53e489c785df13f3618e41dbcd6718c6addbf1395aa6876"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "winnow"
-version = "0.6.6"
+version = "0.6.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f0c976aaaa0e1f90dbb21e9587cdaf1d9679a1cde8875c0d6bd83ab96a208352"
+checksum = "14b9415ee827af173ebb3f15f9083df5a122eb93572ec28741fb153356ea2578"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "winreg"
 version = "0.50.0"
@@ -8329,15 +8363,15 @@
 [[package]]
 name = "x11-clipboard"
 version = "0.9.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b98785a09322d7446e28a13203d2cae1059a0dd3dfb32cb06d0a225f023d8286"
 dependencies = [
  "libc",
- "x11rb 0.13.0",
+ "x11rb 0.13.1",
 ]
 
 [[package]]
 name = "x11-dl"
 version = "2.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "38735924fedd5314a6e548792904ed8c6de6636285cb9fec04d5b1db85c1516f"
@@ -8362,51 +8396,51 @@
  "winapi",
  "winapi-wsapoll",
  "x11rb-protocol 0.12.0",
 ]
 
 [[package]]
 name = "x11rb"
-version = "0.13.0"
+version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f8f25ead8c7e4cba123243a6367da5d3990e0d3affa708ea19dce96356bd9f1a"
+checksum = "5d91ffca73ee7f68ce055750bf9f6eca0780b8c85eff9bc046a3b0da41755e12"
 dependencies = [
  "as-raw-xcb-connection",
  "gethostname 0.4.3",
  "libc",
  "libloading 0.8.3",
  "once_cell",
- "rustix 0.38.32",
- "x11rb-protocol 0.13.0",
+ "rustix 0.38.34",
+ "x11rb-protocol 0.13.1",
 ]
 
 [[package]]
 name = "x11rb-protocol"
 version = "0.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "82d6c3f9a0fb6701fab8f6cea9b0c0bd5d6876f1f89f7fada07e558077c344bc"
 dependencies = [
  "nix 0.26.4",
 ]
 
 [[package]]
 name = "x11rb-protocol"
-version = "0.13.0"
+version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e63e71c4b8bd9ffec2c963173a4dc4cbde9ee96961d4fcb4429db9929b606c34"
+checksum = "ec107c4503ea0b4a98ef47356329af139c0a4f7750e621cf2973cd3385ebcb3d"
 
 [[package]]
 name = "xattr"
 version = "1.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8da84f1a25939b27f6820d92aed108f83ff920fdf11a7b19366c27c4cda81d4f"
 dependencies = [
  "libc",
  "linux-raw-sys 0.4.13",
- "rustix 0.38.32",
+ "rustix 0.38.34",
 ]
 
 [[package]]
 name = "xcursor"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6a0ccd7b4a5345edfcd0c3535718a4e9ff7798ffc536bb5b5a0e26ff84732911"
@@ -8487,15 +8521,15 @@
  "clap",
  "const_format",
  "i-slint-common",
  "lazy_static",
  "proc-macro2",
  "regex",
  "serde_json",
- "toml_edit 0.22.9",
+ "toml_edit 0.22.12",
  "which 6.0.1",
  "xshell",
 ]
 
 [[package]]
 name = "xtensa-atomic-emulation-trap"
 version = "0.4.0"
```

### Comparing `slint-1.6.0a6/Cargo.toml` & `slint-1.6.0a7/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 cbindgen = { version = "0.26", default-features = false }
 css-color-parser2 = { version = "1.0.1" }
 fontdb = { version = "0.16.0", default-features = false }
 fontdue = { version = "0.8.0" }
 glutin = { version = "0.31.1", default-features = false }
 image = { version = "0.24", default-features = false, features = [ "png", "jpeg" ] }
 itertools = { version = "0.12" }
-resvg = { version= "0.40.0", default-features = false, features = ["text"] }
+resvg = { version= "0.41.0", default-features = false, features = ["text"] }
 send_wrapper = { version = "0.6.0" }
 softbuffer = { version = "0.3.3", default-features = false }
 strum = { version = "0.26.1", default-features = false, features = ["derive"] }
 toml_edit = { version = "0.22.7" }
 cfg_aliases = { version = "0.2.0" }
 
 raw-window-handle-06 = { package = "raw-window-handle", version = "0.6", features = ["alloc"] }
```

### Comparing `slint-1.6.0a6/pyproject.toml` & `slint-1.6.0a7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 [build-system]
 requires = ["maturin>=1,<2"]
 build-backend = "maturin"
 
 [project]
 name = "slint"
-version = "1.6.0a6"
+version = "1.6.0a7"
 requires-python = ">= 3.10"
 authors = [
     {name = "Slint Team", email = "info@slint.dev"},
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: MacOS X",
```

### Comparing `slint-1.6.0a6/slint/__init__.py` & `slint-1.6.0a7/slint/__init__.py`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/slint/models.py` & `slint-1.6.0a7/slint/models.py`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a6/PKG-INFO` & `slint-1.6.0a7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: slint
-Version: 1.6.0a6
+Version: 1.6.0a7
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: MacOS X
 Classifier: Environment :: X11 Applications
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Rust
@@ -106,14 +106,15 @@
 ```
 
 1. Create a file called `main.py`:
 
 ```python
 import slint
 
+# slint.loader will look in `sys.path` for `appwindow.slint`.
 class App(slint.loader.appwindow.AppWindow):
     @slint.callback
     def request_increase_value(self):
         self.counter = self.counter + 1
 
 app = App()
 app.run()
```

