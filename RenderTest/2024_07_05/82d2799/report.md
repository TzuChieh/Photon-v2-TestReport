# Render Test Report

* Generation Time (UTC): 2024-07-05 14:25:56.071293+00:00
* 53 cases, 53 passed (100.000000%)
* Total time spent: 2922 seconds

Note that timing is wall-clock time estimated *per-worker*. Depending on the settings, a worker could be a thread or process, etc. If the tests are run in parallel, timing can be higher than its sequential counterpart.

## System Information

* OS: Windows
* CPU: Intel64 Family 6 Model 79 Stepping 1, GenuineIntel (12 logical, 6 physical)
* RAM: 127.913 GiB installed
* Disk: 931.51 GiB total, 426.95 GiB available, 504.55 GiB used

## Failed Tests (0)

All tests passed.

## Passed Tests (53)

* [(3) Test Checkerboard Emissive Quad (50s)](#test-checkerboard-emissive-quad)
* [(7) Test Environment Map (623s)](#test-environment-map)
* [(3) Test Fullscreen Unit Radiance (3s)](#test-fullscreen-unit-radiance)
* [(2) Test Glossy Plane (73s)](#test-glossy-plane)
* [(7) Test Gray Furnace Box (291s)](#test-gray-furnace-box)
* [(5) Test Lerped Lambertian Diffuse (458s)](#test-lerped-lambertian-diffuse)
* [(8) Test Single Ply Mesh (441s)](#test-single-ply-mesh)
* [(7) Test Threading Cornell Box With Gold Sphere (638s)](#test-threading-cornell-box-with-gold-sphere)
* [(2) Test White 100W Point Light (134s)](#test-white-100w-point-light)
* [(3) Test White 100W Rect Area Light (85s)](#test-white-100w-rect-area-light)
* [(2) Test White 100W Small Rect Area Light (15s)](#test-white-100w-small-rect-area-light)
* [(4) Test White 500W Rect Area Light Side (105s)](#test-white-500w-rect-area-light-side)

## Test Checkerboard Emissive Quad

A emissive quad is placed in front of the camera. The emission is textured with a
checkerboard image. The quad will perfectly fit the rendered image (i.e., the rendered output
should be identical to the checkboard image, with a different resolution).

Contains 3 test case(s) (BNEEPT, BVPT, SPPM).

### (1/3) Case BNEEPT: *\<PASSED\>*

Time spent: 27 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_checkerboard_emissive_quad/bneept.jpg)    |      ![reference image](tests.test_checkerboard_emissive_quad/ref.jpg)     |

#### Debug Output

![debug output image](tests.test_checkerboard_emissive_quad/bneept_error.jpg)

### (2/3) Case BVPT: *\<PASSED\>*

Time spent: 14 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_checkerboard_emissive_quad/bvpt.jpg)    |      ![reference image](tests.test_checkerboard_emissive_quad/ref.jpg)     |

#### Debug Output

![debug output image](tests.test_checkerboard_emissive_quad/bvpt_error.jpg)

### (3/3) Case SPPM: *\<PASSED\>*

Time spent: 8 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_checkerboard_emissive_quad/sppm.jpg)    |      ![reference image](tests.test_checkerboard_emissive_quad/ref.jpg)     |

#### Debug Output

![debug output image](tests.test_checkerboard_emissive_quad/sppm_error.jpg)

## Test Environment Map

An object is being illuminated by an environment map.

Contains 7 test case(s) (BNEEPT (debug map + sphere + shifted), BNEEPT (debug map + sphere), BNEEPT (white map + sphere), BVPT (debug map + sphere + shifted), BVPT (debug map + sphere), BVPT (white map + sphere), PPPM (white map + plane)).

### (1/7) Case BNEEPT (debug map + sphere + shifted): *\<PASSED\>*

All settings are the same with "BNEEPT (debug map + sphere)" case, except the sphere and camera are shifted 2000 units in +x. The result should be the same as our environment map depends on view direction only.

Time spent: 17 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_environment_map/debug_bneept_sphere_shifted.jpg)    |      ![reference image](tests.test_environment_map/ref_debug_sphere.jpg)     |

#### Debug Output

![debug output image](tests.test_environment_map/debug_bneept_sphere_shifted_error.jpg)

### (2/7) Case BNEEPT (debug map + sphere): *\<PASSED\>*

Time spent: 24 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_environment_map/debug_bneept_sphere.jpg)    |      ![reference image](tests.test_environment_map/ref_debug_sphere.jpg)     |

#### Debug Output

![debug output image](tests.test_environment_map/debug_bneept_sphere_error.jpg)

### (3/7) Case BNEEPT (white map + sphere): *\<PASSED\>*

Effectively a white furnace test.

Time spent: 5 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_environment_map/white_bneept_sphere.jpg)    |      ![reference image](tests.test_environment_map/ref_white.jpg)     |

#### Debug Output

![debug output image](tests.test_environment_map/white_bneept_sphere_error.jpg)

### (4/7) Case BVPT (debug map + sphere + shifted): *\<PASSED\>*

All settings are the same with "BVPT (debug map + sphere)" case, except the sphere and camera are shifted 2000 units in +x. The result should be the same as our environment map depends on view direction only.

Time spent: 12 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_environment_map/debug_bvpt_sphere_shifted.jpg)    |      ![reference image](tests.test_environment_map/ref_debug_sphere.jpg)     |

#### Debug Output

![debug output image](tests.test_environment_map/debug_bvpt_sphere_shifted_error.jpg)

### (5/7) Case BVPT (debug map + sphere): *\<PASSED\>*

Time spent: 13 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_environment_map/debug_bvpt_sphere.jpg)    |      ![reference image](tests.test_environment_map/ref_debug_sphere.jpg)     |

#### Debug Output

![debug output image](tests.test_environment_map/debug_bvpt_sphere_error.jpg)

### (6/7) Case BVPT (white map + sphere): *\<PASSED\>*

Effectively a white furnace test.

Time spent: 3 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_environment_map/white_bvpt_sphere.jpg)    |      ![reference image](tests.test_environment_map/ref_white.jpg)     |

#### Debug Output

![debug output image](tests.test_environment_map/white_bvpt_sphere_error.jpg)

### (7/7) Case PPPM (white map + plane): *\<PASSED\>*

Effectively a white furnace test. The receiver is placed fairly close to the plane, looking at the horizon (forms grazing angles). The environment sphere is also shifted and rotated, which should not affect the result.

Time spent: 546 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_environment_map/white_pppm_plane.jpg)    |      ![reference image](tests.test_environment_map/ref_white.jpg)     |

#### Debug Output

![debug output image](tests.test_environment_map/white_pppm_plane_error.jpg)

## Test Fullscreen Unit Radiance

These scenes are all arranged in a way that they should render as a frame filled with
white of unit magnitude (1, 1, 1). All output images should appear white, and all images showing
error should be completely black (or any other color representing 0, depending on the color map).

Contains 3 test case(s) (BNEEPT, BVPT, SPPM).

### (1/3) Case BNEEPT: *\<PASSED\>*

Time spent: 2 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_fullscreen_unit_radiance/bneept.jpg)    |      (no reference image)     |

#### Debug Output

![debug output image](tests.test_fullscreen_unit_radiance/bneept_error.jpg)

### (2/3) Case BVPT: *\<PASSED\>*

Time spent: 0 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_fullscreen_unit_radiance/bvpt.jpg)    |      (no reference image)     |

#### Debug Output

![debug output image](tests.test_fullscreen_unit_radiance/bvpt_error.jpg)

### (3/3) Case SPPM: *\<PASSED\>*

Time spent: 0 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_fullscreen_unit_radiance/sppm.jpg)    |      (no reference image)     |

#### Debug Output

![debug output image](tests.test_fullscreen_unit_radiance/sppm_error.jpg)

## Test Glossy Plane

A glossy plane is being illuminated by an average size area light. This scene is modeled and exported
from Blender. Expected to see glossy appearance clearly.

Contains 2 test case(s) (BNEEPT, BVPT).

### (1/2) Case BNEEPT: *\<PASSED\>*

Time spent: 34 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_glossy_plane/bneept.jpg)    |      ![reference image](tests.test_glossy_plane/ref.jpg)     |

#### Debug Output

![debug output image](tests.test_glossy_plane/bneept_error.jpg)

### (2/2) Case BVPT: *\<PASSED\>*

Time spent: 39 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_glossy_plane/bvpt.jpg)    |      ![reference image](tests.test_glossy_plane/ref.jpg)     |

#### Debug Output

![debug output image](tests.test_glossy_plane/bvpt_error.jpg)

## Test Gray Furnace Box

The classical white furnace test, with medium gray background to better judge energy loss/gain. There is
an object placed in the middle. If there is no energy loss in the target model, then the output image
should be 0.5 for all pixels.

Contains 7 test case(s) (BNEEPT Diffuse Sphere, BNEEPT Diffuse Sphere (Small Box), BNEEPT Glass Cube, BNEEPT Glass Sphere, BVPT Diffuse Sphere, PPPM Glass Cube, SPPM Diffuse Sphere).

### (1/7) Case BNEEPT Diffuse Sphere: *\<PASSED\>*

Time spent: 36 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_gray_furnace_box/bneept_diffuse_sphere.jpg)    |      (no reference image)     |

#### Debug Output

![debug output image](tests.test_gray_furnace_box/bneept_diffuse_sphere_error.jpg)

Debug message: mean diff = 0.00007248, max pixel = 0.50902522, min pixel = 0.49090388

### (2/7) Case BNEEPT Diffuse Sphere (Small Box): *\<PASSED\>*

All settings are the same with "BNEEPT Diffuse Sphere" case, except the furnace is a smaller box (2000 -> 40, 50X reduction).

Time spent: 40 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_gray_furnace_box/bneept_diffuse_sphere_small_box.jpg)    |      (no reference image)     |

#### Debug Output

![debug output image](tests.test_gray_furnace_box/bneept_diffuse_sphere_small_box_error.jpg)

Debug message: mean diff = 0.00002887, max pixel = 0.50608510, min pixel = 0.49324462

### (3/7) Case BNEEPT Glass Cube: *\<PASSED\>*

Time spent: 44 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_gray_furnace_box/bneept_glass_cube.jpg)    |      (no reference image)     |

#### Debug Output

![debug output image](tests.test_gray_furnace_box/bneept_glass_cube_error.jpg)

Debug message: mean diff = -0.00000830, max pixel = 0.50913209, min pixel = 0.49223518

### (4/7) Case BNEEPT Glass Sphere: *\<PASSED\>*

Time spent: 14 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_gray_furnace_box/bneept_glass_sphere.jpg)    |      (no reference image)     |

#### Debug Output

![debug output image](tests.test_gray_furnace_box/bneept_glass_sphere_error.jpg)

Debug message: mean diff = -0.00001011, max pixel = 0.50519168, min pixel = 0.49506178

### (5/7) Case BVPT Diffuse Sphere: *\<PASSED\>*

Time spent: 9 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_gray_furnace_box/bvpt_diffuse_sphere.jpg)    |      (no reference image)     |

#### Debug Output

![debug output image](tests.test_gray_furnace_box/bvpt_diffuse_sphere_error.jpg)

Debug message: mean diff = 0.00000000, max pixel = 0.50000000, min pixel = 0.50000000

### (6/7) Case PPPM Glass Cube: *\<PASSED\>*

Time spent: 21 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_gray_furnace_box/pppm_glass_cube.jpg)    |      (no reference image)     |

#### Debug Output

![debug output image](tests.test_gray_furnace_box/pppm_glass_cube_error.jpg)

Debug message: mean diff = -0.00001708, max pixel = 0.56971490, min pixel = 0.44924352

### (7/7) Case SPPM Diffuse Sphere: *\<PASSED\>*

Time spent: 124 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_gray_furnace_box/sppm_diffuse_sphere.jpg)    |      (no reference image)     |

#### Debug Output

![debug output image](tests.test_gray_furnace_box/sppm_diffuse_sphere_error.jpg)

Debug message: mean diff = 0.00026006, max pixel = 0.57694024, min pixel = 0.43489695

## Test Lerped Lambertian Diffuse

A sphere with lerped Lambertian diffuse of different factors, comparing against a non-lerped (albedo = 
100%) reference. The ground is non-lerped diffusive (albedo = 50%).

Contains 5 test case(s) (BNEEPT (factor = 0 percent), BNEEPT (factor = 50 percent), BVPT (factor = 0 percent), BVPT (factor = 50 percent), BVPT (factor = 80 percent)).

### (1/5) Case BNEEPT (factor = 0 percent): *\<PASSED\>*

This is a corner case where the lerping factor is 0 (0 * material_0 + 1 * material_0).

Time spent: 135 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_lerped_lambertian_diffuse/bneept_factor0p0.jpg)    |      ![reference image](tests.test_lerped_lambertian_diffuse/ref.jpg)     |

#### Debug Output

![debug output image](tests.test_lerped_lambertian_diffuse/bneept_factor0p0_error.jpg)

### (2/5) Case BNEEPT (factor = 50 percent): *\<PASSED\>*

Time spent: 118 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_lerped_lambertian_diffuse/bneept_factor0p5.jpg)    |      ![reference image](tests.test_lerped_lambertian_diffuse/ref.jpg)     |

#### Debug Output

![debug output image](tests.test_lerped_lambertian_diffuse/bneept_factor0p5_error.jpg)

### (3/5) Case BVPT (factor = 0 percent): *\<PASSED\>*

This is a corner case where the lerping factor is 0 (0 * material_0 + 1 * material_0).

Time spent: 65 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_lerped_lambertian_diffuse/bvpt_factor0p0.jpg)    |      ![reference image](tests.test_lerped_lambertian_diffuse/ref.jpg)     |

#### Debug Output

![debug output image](tests.test_lerped_lambertian_diffuse/bvpt_factor0p0_error.jpg)

### (4/5) Case BVPT (factor = 50 percent): *\<PASSED\>*

Time spent: 71 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_lerped_lambertian_diffuse/bvpt_factor0p5.jpg)    |      ![reference image](tests.test_lerped_lambertian_diffuse/ref.jpg)     |

#### Debug Output

![debug output image](tests.test_lerped_lambertian_diffuse/bvpt_factor0p5_error.jpg)

### (5/5) Case BVPT (factor = 80 percent): *\<PASSED\>*

Time spent: 67 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_lerped_lambertian_diffuse/bvpt_factor0p8.jpg)    |      ![reference image](tests.test_lerped_lambertian_diffuse/ref.jpg)     |

#### Debug Output

![debug output image](tests.test_lerped_lambertian_diffuse/bvpt_factor0p8_error.jpg)

## Test Single Ply Mesh

A single .ply mesh is placed between a large area light and diffusive ground. The mesh itself is diffusive.

Contains 8 test case(s) (Quad (BNEEPT), Quad (BNEEPT, ASCII), Quad (BVPT), Quad (BVPT, ASCII), Quad (SPPM), Suzanne (BNEEPT), Suzanne (BVPT), Suzanne (SPPM)).

### (1/8) Case Quad (BNEEPT): *\<PASSED\>*

Time spent: 14 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_single_ply_mesh/quad_bneept.jpg)    |      ![reference image](tests.test_single_ply_mesh/ref_quad.jpg)     |

#### Debug Output

![debug output image](tests.test_single_ply_mesh/quad_bneept_error.jpg)

### (2/8) Case Quad (BNEEPT, ASCII): *\<PASSED\>*

Time spent: 11 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_single_ply_mesh/quad_bneept_ascii.jpg)    |      ![reference image](tests.test_single_ply_mesh/ref_quad.jpg)     |

#### Debug Output

![debug output image](tests.test_single_ply_mesh/quad_bneept_ascii_error.jpg)

### (3/8) Case Quad (BVPT): *\<PASSED\>*

Time spent: 4 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_single_ply_mesh/quad_bvpt.jpg)    |      ![reference image](tests.test_single_ply_mesh/ref_quad.jpg)     |

#### Debug Output

![debug output image](tests.test_single_ply_mesh/quad_bvpt_error.jpg)

### (4/8) Case Quad (BVPT, ASCII): *\<PASSED\>*

Time spent: 7 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_single_ply_mesh/quad_bvpt_ascii.jpg)    |      ![reference image](tests.test_single_ply_mesh/ref_quad.jpg)     |

#### Debug Output

![debug output image](tests.test_single_ply_mesh/quad_bvpt_ascii_error.jpg)

### (5/8) Case Quad (SPPM): *\<PASSED\>*

Time spent: 161 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_single_ply_mesh/quad_sppm.jpg)    |      ![reference image](tests.test_single_ply_mesh/ref_quad.jpg)     |

#### Debug Output

![debug output image](tests.test_single_ply_mesh/quad_sppm_error.jpg)

### (6/8) Case Suzanne (BNEEPT): *\<PASSED\>*

Time spent: 25 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_single_ply_mesh/suzanne_bneept.jpg)    |      ![reference image](tests.test_single_ply_mesh/ref_suzanne.jpg)     |

#### Debug Output

![debug output image](tests.test_single_ply_mesh/suzanne_bneept_error.jpg)

### (7/8) Case Suzanne (BVPT): *\<PASSED\>*

Time spent: 14 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_single_ply_mesh/suzanne_bvpt.jpg)    |      ![reference image](tests.test_single_ply_mesh/ref_suzanne.jpg)     |

#### Debug Output

![debug output image](tests.test_single_ply_mesh/suzanne_bvpt_error.jpg)

### (8/8) Case Suzanne (SPPM): *\<PASSED\>*

Time spent: 200 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_single_ply_mesh/suzanne_sppm.jpg)    |      ![reference image](tests.test_single_ply_mesh/ref_suzanne.jpg)     |

#### Debug Output

![debug output image](tests.test_single_ply_mesh/suzanne_sppm_error.jpg)

## Test Threading Cornell Box With Gold Sphere

This test is for testing threaded rendering on a simple scene.

Contains 7 test case(s) (BNEEPT (1) 1T, BNEEPT (2) 2T, BNEEPT (3) 5T, BNEEPT (4) 8T, BNEEPT (5) 17T, BNEEPT (6) 64T, BNEEPT (7) 100T).

### (1/7) Case BNEEPT (1) 1T: *\<PASSED\>*

Time spent: 172 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_threading_cornell_box_with_gold_sphere/bneept_1t.jpg)    |      ![reference image](tests.test_threading_cornell_box_with_gold_sphere/ref.jpg)     |

#### Debug Output

![debug output image](tests.test_threading_cornell_box_with_gold_sphere/bneept_error_1t.jpg)

### (2/7) Case BNEEPT (2) 2T: *\<PASSED\>*

Time spent: 231 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_threading_cornell_box_with_gold_sphere/bneept_2t.jpg)    |      ![reference image](tests.test_threading_cornell_box_with_gold_sphere/ref.jpg)     |

#### Debug Output

![debug output image](tests.test_threading_cornell_box_with_gold_sphere/bneept_error_2t.jpg)

### (3/7) Case BNEEPT (3) 5T: *\<PASSED\>*

Time spent: 75 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_threading_cornell_box_with_gold_sphere/bneept_5t.jpg)    |      ![reference image](tests.test_threading_cornell_box_with_gold_sphere/ref.jpg)     |

#### Debug Output

![debug output image](tests.test_threading_cornell_box_with_gold_sphere/bneept_error_5t.jpg)

### (4/7) Case BNEEPT (4) 8T: *\<PASSED\>*

Time spent: 75 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_threading_cornell_box_with_gold_sphere/bneept_8t.jpg)    |      ![reference image](tests.test_threading_cornell_box_with_gold_sphere/ref.jpg)     |

#### Debug Output

![debug output image](tests.test_threading_cornell_box_with_gold_sphere/bneept_error_8t.jpg)

### (5/7) Case BNEEPT (5) 17T: *\<PASSED\>*

Time spent: 28 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_threading_cornell_box_with_gold_sphere/bneept_17t.jpg)    |      ![reference image](tests.test_threading_cornell_box_with_gold_sphere/ref.jpg)     |

#### Debug Output

![debug output image](tests.test_threading_cornell_box_with_gold_sphere/bneept_error_17t.jpg)

### (6/7) Case BNEEPT (6) 64T: *\<PASSED\>*

Time spent: 26 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_threading_cornell_box_with_gold_sphere/bneept_64t.jpg)    |      ![reference image](tests.test_threading_cornell_box_with_gold_sphere/ref.jpg)     |

#### Debug Output

![debug output image](tests.test_threading_cornell_box_with_gold_sphere/bneept_error_64t.jpg)

### (7/7) Case BNEEPT (7) 100T: *\<PASSED\>*

Time spent: 28 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_threading_cornell_box_with_gold_sphere/bneept_100t.jpg)    |      ![reference image](tests.test_threading_cornell_box_with_gold_sphere/ref.jpg)     |

#### Debug Output

![debug output image](tests.test_threading_cornell_box_with_gold_sphere/bneept_error_100t.jpg)

## Test White 100W Point Light

This test is similar to the "white_100W_small_rect_area_light" test, except that we are using a
point light here. In Photon, we do not have true point light, they are just tiny spherical light.
This test is not suitable to run using BVPT, as it may require way more than 10M samples to have
proper convergence.

Contains 2 test case(s) (BNEEPT, SPPM).

### (1/2) Case BNEEPT: *\<PASSED\>*

Time spent: 98 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_white_100W_point_light/bneept.jpg)    |      ![reference image](tests.test_white_100W_point_light/ref.jpg)     |

#### Debug Output

![debug output image](tests.test_white_100W_point_light/bneept_error.jpg)

### (2/2) Case SPPM: *\<PASSED\>*

Time spent: 35 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_white_100W_point_light/sppm.jpg)    |      ![reference image](tests.test_white_100W_point_light/ref.jpg)     |

#### Debug Output

![debug output image](tests.test_white_100W_point_light/sppm_error.jpg)

## Test White 100W Rect Area Light

A rectangular area light is shining the ground below it. The ground is diffusive (albedo = 50%).

Contains 3 test case(s) (BNEEPT, BVPT, SPPM).

### (1/3) Case BNEEPT: *\<PASSED\>*

Time spent: 57 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_white_100W_rect_area_light/bneept.jpg)    |      ![reference image](tests.test_white_100W_rect_area_light/ref.jpg)     |

#### Debug Output

![debug output image](tests.test_white_100W_rect_area_light/bneept_error.jpg)

### (2/3) Case BVPT: *\<PASSED\>*

Time spent: 22 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_white_100W_rect_area_light/bvpt.jpg)    |      ![reference image](tests.test_white_100W_rect_area_light/ref.jpg)     |

#### Debug Output

![debug output image](tests.test_white_100W_rect_area_light/bvpt_error.jpg)

### (3/3) Case SPPM: *\<PASSED\>*

Time spent: 5 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_white_100W_rect_area_light/sppm.jpg)    |      ![reference image](tests.test_white_100W_rect_area_light/ref.jpg)     |

#### Debug Output

![debug output image](tests.test_white_100W_rect_area_light/sppm_error.jpg)

## Test White 100W Small Rect Area Light

This test is similar to the "white_100W_rect_area_light" test, except that the rectangular
area light is much smaller (0.005 x 0.005 unit^2), and the light source is placed higher above the
ground so it cannot induce too much variance (it is a strong radiance source). This test is not
suitable to run using  BVPT, as it may require way more than 10M samples to have proper convergence.

Contains 2 test case(s) (BNEEPT, SPPM).

### (1/2) Case BNEEPT: *\<PASSED\>*

Time spent: 8 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_white_100W_small_rect_area_light/bneept.jpg)    |      ![reference image](tests.test_white_100W_small_rect_area_light/ref.jpg)     |

#### Debug Output

![debug output image](tests.test_white_100W_small_rect_area_light/bneept_error.jpg)

### (2/2) Case SPPM: *\<PASSED\>*

Time spent: 6 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_white_100W_small_rect_area_light/sppm.jpg)    |      ![reference image](tests.test_white_100W_small_rect_area_light/ref.jpg)     |

#### Debug Output

![debug output image](tests.test_white_100W_small_rect_area_light/sppm_error.jpg)

## Test White 500W Rect Area Light Side

This test places a bigger rectangular area light on the left, and objects of different materials are being
illuminated. Since the light is quite large, all rendering methods should be able to perform this test.

Contains 4 test case(s) (BNEEPT Diffuse Sphere, BNEEPT Glass Sphere, BVPT Diffuse Sphere, BVPT Glass Sphere).

### (1/4) Case BNEEPT Diffuse Sphere: *\<PASSED\>*

Time spent: 13 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_white_500W_rect_area_light_side/bneept_diffuse_sphere.jpg)    |      ![reference image](tests.test_white_500W_rect_area_light_side/ref_diffuse_sphere.jpg)     |

#### Debug Output

![debug output image](tests.test_white_500W_rect_area_light_side/bneept_diffuse_sphere_error.jpg)

### (2/4) Case BNEEPT Glass Sphere: *\<PASSED\>*

Time spent: 40 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_white_500W_rect_area_light_side/bneept_glass_sphere.jpg)    |      ![reference image](tests.test_white_500W_rect_area_light_side/ref_glass_sphere.jpg)     |

#### Debug Output

![debug output image](tests.test_white_500W_rect_area_light_side/bneept_glass_sphere_error.jpg)

### (3/4) Case BVPT Diffuse Sphere: *\<PASSED\>*

Time spent: 20 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_white_500W_rect_area_light_side/bvpt_diffuse_sphere.jpg)    |      ![reference image](tests.test_white_500W_rect_area_light_side/ref_diffuse_sphere.jpg)     |

#### Debug Output

![debug output image](tests.test_white_500W_rect_area_light_side/bvpt_diffuse_sphere_error.jpg)

### (4/4) Case BVPT Glass Sphere: *\<PASSED\>*

Time spent: 31 seconds.

|  Output  |  Reference  |
| :------: | :---------: |
|    ![output image](tests.test_white_500W_rect_area_light_side/bvpt_glass_sphere.jpg)    |      ![reference image](tests.test_white_500W_rect_area_light_side/ref_glass_sphere.jpg)     |

#### Debug Output

![debug output image](tests.test_white_500W_rect_area_light_side/bvpt_glass_sphere_error.jpg)

