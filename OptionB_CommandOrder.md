# First non-pyjoules except for helix spin, then pyjoules except for helix spin. Separately after we'll do helix spin with and without pyjoules.


## Part 1: All Non-PyJoules Except Helix Spin

```bash
ros2 run newton_raphson_enhanced run --platform hw --trajectory hover --double-speed --hover-mode 1 --log-file hw_nr_enh_hover_2x.csv
ros2 run newton_raphson_enhanced run --platform hw --trajectory yaw_only --double-speed --log-file hw_nr_enh_yaw_only_2x.csv
ros2 run newton_raphson_enhanced run --platform hw --trajectory circle_horz --double-speed --log-file hw_nr_enh_circle_horz_2x.csv
ros2 run newton_raphson_enhanced run --platform hw --trajectory circle_horz --double-speed --spin --log-file hw_nr_enh_circle_horz_2x_spin.csv
ros2 run newton_raphson_enhanced run --platform hw --trajectory circle_vert --double-speed --log-file hw_nr_enh_circle_vert_2x.csv
ros2 run newton_raphson_enhanced run --platform hw --trajectory fig8_horz --double-speed --log-file hw_nr_enh_fig8_horz_2x.csv
ros2 run newton_raphson_enhanced run --platform hw --trajectory fig8_vert --double-speed --log-file hw_nr_enh_fig8_vert_2x.csv
ros2 run newton_raphson_enhanced run --platform hw --trajectory fig8_vert --double-speed --short --log-file hw_nr_enh_fig8_vert_2x_short.csv
ros2 run newton_raphson_enhanced run --platform hw --trajectory helix --double-speed --log-file hw_nr_enh_helix_2x.csv
ros2 run newton_raphson_enhanced run --platform hw --trajectory sawtooth --double-speed --log-file hw_nr_enh_sawtooth_2x.csv
ros2 run newton_raphson_enhanced run --platform hw --trajectory triangle --double-speed --log-file hw_nr_enh_triangle_2x.csv
```


## Part 2: All PyJoules Except Helix Spin

```bash
ros2 run newton_raphson_enhanced run --platform hw --trajectory hover --double-speed --hover-mode 1 --pyjoules --log-file hw_nr_enh_hover_2x_pyj.csv
ros2 run newton_raphson_enhanced run --platform hw --trajectory yaw_only --double-speed --pyjoules --log-file hw_nr_enh_yaw_only_2x_pyj.csv
ros2 run newton_raphson_enhanced run --platform hw --trajectory circle_horz --double-speed --pyjoules --log-file hw_nr_enh_circle_horz_2x_pyj.csv
ros2 run newton_raphson_enhanced run --platform hw --trajectory circle_horz --double-speed --spin --pyjoules --log-file hw_nr_enh_circle_horz_2x_spin_pyj.csv
ros2 run newton_raphson_enhanced run --platform hw --trajectory circle_vert --double-speed --pyjoules --log-file hw_nr_enh_circle_vert_2x_pyj.csv
ros2 run newton_raphson_enhanced run --platform hw --trajectory fig8_horz --double-speed --pyjoules --log-file hw_nr_enh_fig8_horz_2x_pyj.csv
ros2 run newton_raphson_enhanced run --platform hw --trajectory fig8_vert --double-speed --pyjoules --log-file hw_nr_enh_fig8_vert_2x_pyj.csv
ros2 run newton_raphson_enhanced run --platform hw --trajectory fig8_vert --double-speed --short --pyjoules --log-file hw_nr_enh_fig8_vert_2x_short_pyj.csv
ros2 run newton_raphson_enhanced run --platform hw --trajectory helix --double-speed --pyjoules --log-file hw_nr_enh_helix_2x_pyj.csv
ros2 run newton_raphson_enhanced run --platform hw --trajectory sawtooth --double-speed --pyjoules --log-file hw_nr_enh_sawtooth_2x_pyj.csv
ros2 run newton_raphson_enhanced run --platform hw --trajectory triangle --double-speed --pyjoules --log-file hw_nr_enh_triangle_2x_pyj.csv
```



## Part 3: Helix Spin with and without PyJoules

```bash
ros2 run newton_raphson_enhanced run --platform hw --trajectory helix --double-speed --spin --log-file hw_nr_enh_helix_2x_spin.csv
ros2 run newton_raphson_enhanced run --platform hw --trajectory helix --double-speed --spin --pyjoules --log-file hw_nr_enh_helix_2x_spin_pyj.csv
```