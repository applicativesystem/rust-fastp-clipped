# rust-window-clipped

- rust implementation of the tilled window approach for dropping the adapters.
- instead of looking at each base, scans the read using the length of the adapter so that it becomes fast iterative. 
- first drops the bases and then uses a iteration to clip the reads with in memory and no read and write multiple times.

```
cargo build

```
- how to run the binary

```
λ gauravsablok rust-fastp-clipped → λ git main* → ./target/debug/rust-window-clipped -h
Usage: rust-window-clipped <READS_1_ARG> <READS_2_ARG> <QUALITY_SCORE> <ADAPTER_ARG>

Arguments:
  <READS_1_ARG>    please provide the reads R1 file path
  <READS_2_ARG>    please provide the reads R2 file path
  <QUALITY_SCORE>  please provide the quality value to be used as a threshold
  <ADAPTER_ARG>    please provide the adapter sequence

Options:
  -h, --help     Print help
  -V, --version  Print version

```

Gaurav Sablok
