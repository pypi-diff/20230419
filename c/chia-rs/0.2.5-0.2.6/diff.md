# Comparing `tmp/chia_rs-0.2.5.tar.gz` & `tmp/chia_rs-0.2.6.tar.gz`

## Comparing `chia_rs-0.2.5.tar` & `chia_rs-0.2.6.tar`

### file list

```diff
@@ -1,136 +1,136 @@
--rw-r--r--   0        0        0      470 1970-01-01 00:00:00.000000 chia_rs-0.2.5/local_dependencies/chia_streamable_macro/Cargo.toml
--rw-r--r--   0     1001      123     4715 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia_streamable_macro/src/lib.rs
--rw-r--r--   0        0        0      458 1970-01-01 00:00:00.000000 chia_rs-0.2.5/local_dependencies/chia_py_streamable_macro/Cargo.toml
--rw-r--r--   0     1001      123     9330 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia_py_streamable_macro/src/lib.rs
--rw-r--r--   0        0        0      781 1970-01-01 00:00:00.000000 chia_rs-0.2.5/local_dependencies/chia-protocol/Cargo.toml
--rw-r--r--   0     1001      123      722 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia-protocol/src/bls.rs
--rw-r--r--   0     1001      123     5474 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia-protocol/src/bytes.rs
--rw-r--r--   0     1001      123     1386 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia-protocol/src/chia_error.rs
--rw-r--r--   0     1001      123     4701 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia-protocol/src/chia_protocol.rs
--rw-r--r--   0     1001      123      862 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia-protocol/src/classgroup.rs
--rw-r--r--   0     1001      123     1809 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia-protocol/src/coin.rs
--rw-r--r--   0     1001      123      556 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia-protocol/src/coin_spend.rs
--rw-r--r--   0     1001      123      540 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia-protocol/src/coin_state.rs
--rw-r--r--   0     1001      123      743 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia-protocol/src/end_of_sub_slot_bundle.rs
--rw-r--r--   0     1001      123      871 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia-protocol/src/fee_estimate.rs
--rw-r--r--   0     1001      123     2316 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia-protocol/src/foliage.rs
--rw-r--r--   0     1001      123     3679 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia-protocol/src/from_json_dict.rs
--rw-r--r--   0     1001      123     1497 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia-protocol/src/fullblock.rs
--rw-r--r--   0     1001      123     1388 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia-protocol/src/header_block.rs
--rw-r--r--   0     1001      123     1288 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia-protocol/src/lib.rs
--rw-r--r--   0     1001      123      810 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia-protocol/src/message_struct.rs
--rw-r--r--   0     1001      123      540 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia-protocol/src/pool_target.rs
--rw-r--r--   0     1001      123     1624 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia-protocol/src/program.rs
--rw-r--r--   0     1001      123      679 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia-protocol/src/proof_of_space.rs
--rw-r--r--   0     1001      123     1527 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia-protocol/src/reward_chain_block.rs
--rw-r--r--   0     1001      123     1788 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia-protocol/src/slots.rs
--rw-r--r--   0     1001      123      569 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia-protocol/src/spend_bundle.rs
--rw-r--r--   0     1001      123    20212 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia-protocol/src/streamable.rs
--rw-r--r--   0     1001      123     2217 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia-protocol/src/to_json_dict.rs
--rw-r--r--   0     1001      123      679 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia-protocol/src/vdf.rs
--rw-r--r--   0     1001      123     4016 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia-protocol/src/wallet_protocol.rs
--rw-r--r--   0     1001      123     1225 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia-protocol/src/weight_proof.rs
--rw-r--r--   0        0        0     1001 1970-01-01 00:00:00.000000 chia_rs-0.2.5/local_dependencies/chia/Cargo.toml
--rw-r--r--   0     1001      123      224 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/.cargo/config
--rw-r--r--   0     1001      123      290 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/.github/workflows/audit-check.yml
--rw-r--r--   0     1001      123     3050 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/.github/workflows/benchmark.yml
--rw-r--r--   0     1001      123     2843 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/.github/workflows/build-crate-and-npm.yml
--rw-r--r--   0     1001      123    13503 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/.github/workflows/build-test.yml
--rw-r--r--   0     1001      123       19 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/.gitignore
--rw-r--r--   0     1001      123    11357 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/LICENSE
--rw-r--r--   0     1001      123      192 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/README.md
--rw-r--r--   0     1001      123      142 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/cl/README.md
--rw-r--r--   0     1001      123     4603 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/cl/deserialize_w_backrefs.cl
--rw-r--r--   0     1001      123     4474 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/docs/implementation-notes.md
--rw-r--r--   0     1001      123      882 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/examples/README.md
--rw-r--r--   0     1001      123    48843 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/examples/block-1519806.bin
--rw-r--r--   0     1001      123      299 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/examples/dump.py
--rw-r--r--   0     1001      123     1592 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/examples/streaming-patch.diff
--rw-r--r--   0     1001      123       93 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/mypy.ini
--rw-r--r--   0     1001      123      261 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/src/allocator.rs
--rw-r--r--   0     1001      123     1817 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/src/compression/compressor.rs
--rw-r--r--   0     1001      123      858 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/src/compression/deserialize_w_backrefs.bin
--rw-r--r--   0     1001      123       20 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/src/compression/mod.rs
--rw-r--r--   0     1001      123     3120 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/src/fuzzing_utils.rs
--rw-r--r--   0     1001      123     3042 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/src/gen/coin_id.rs
--rw-r--r--   0     1001      123     4493 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/src/gen/condition_sanitizers.rs
--rw-r--r--   0     1001      123   129755 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/src/gen/conditions.rs
--rw-r--r--   0     1001      123      972 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/src/gen/flags.rs
--rw-r--r--   0     1001      123     6447 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/src/gen/get_puzzle_and_solution.rs
--rw-r--r--   0     1001      123      221 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/src/gen/mod.rs
--rw-r--r--   0     1001      123     7075 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/src/gen/opcodes.rs
--rw-r--r--   0     1001      123     2305 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/src/gen/run_block_generator.rs
--rw-r--r--   0     1001      123     2159 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/src/gen/run_puzzle.rs
--rw-r--r--   0     1001      123     2916 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/src/gen/sanitize_int.rs
--rw-r--r--   0     1001      123     5743 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/src/gen/validation_error.rs
--rw-r--r--   0     1001      123     4972 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/src/generator_rom.rs
--rw-r--r--   0     1001      123      136 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/src/lib.rs
--rw-r--r--   0     1001      123    22862 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/src/merkle_set.rs
--rwxr-xr-x   0     1001      123     8264 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/tests/generate-programs.py
--rw-r--r--   0     1001      123     1143 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/tests/generators/assert-puzzle-announce-fail.clvm
--rw-r--r--   0     1001      123    21116 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/tests/generators/block-834752.clvm
--rw-r--r--   0     1001      123    25761 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/tests/generators/block-834752.hex
--rw-r--r--   0     1001      123    99972 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/tests/generators/block-834760.clvm
--rw-r--r--   0     1001      123    22001 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/tests/generators/block-834761.clvm
--rw-r--r--   0     1001      123    59172 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/tests/generators/block-834765.clvm
--rw-r--r--   0     1001      123   105717 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/tests/generators/block-834766.clvm
--rw-r--r--   0     1001      123    83316 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/tests/generators/block-834768.clvm
--rw-r--r--   0     1001      123      577 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/tests/generators/create-coin-different-amounts.clvm
--rw-r--r--   0     1001      123      267 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/tests/generators/create-coin-hint-duplicate-outputs.clvm
--rw-r--r--   0     1001      123      685 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/tests/generators/create-coin-hint.clvm
--rw-r--r--   0     1001      123      699 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/tests/generators/create-coin-hint2.clvm
--rw-r--r--   0     1001      123      456 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/tests/generators/deep-recursion-plus.clvm
--rw-r--r--   0     1001      123      382 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/tests/generators/double-spend.clvm
--rw-r--r--   0     1001      123      501 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/tests/generators/duplicate-coin-announce.clvm
--rw-r--r--   0     1001      123      263 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/tests/generators/duplicate-create-coin.clvm
--rw-r--r--   0     1001      123      448 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/tests/generators/duplicate-height-absolute-div.clvm
--rw-r--r--   0     1001      123      429 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/tests/generators/duplicate-height-absolute-substr-tail.clvm
--rw-r--r--   0     1001      123      422 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/tests/generators/duplicate-height-absolute-substr.clvm
--rw-r--r--   0     1001      123      391 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/tests/generators/duplicate-height-absolute.clvm
--rw-r--r--   0     1001      123      391 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/tests/generators/duplicate-height-relative.clvm
--rw-r--r--   0     1001      123      196 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/tests/generators/duplicate-outputs.clvm
--rw-r--r--   0     1001      123      391 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/tests/generators/duplicate-reserve-fee.clvm
--rw-r--r--   0     1001      123      391 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/tests/generators/duplicate-seconds-absolute.clvm
--rw-r--r--   0     1001      123      392 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/tests/generators/duplicate-seconds-relative.clvm
--rw-r--r--   0     1001      123      380 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/tests/generators/height-absolute-ladder.clvm
--rw-r--r--   0     1001      123      104 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/tests/generators/infinite-recursion1.clvm
--rw-r--r--   0     1001      123       92 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/tests/generators/infinite-recursion2.clvm
--rw-r--r--   0     1001      123     1458 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/tests/generators/infinite-recursion3.clvm
--rw-r--r--   0     1001      123      160 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/tests/generators/infinite-recursion4.clvm
--rw-r--r--   0     1001      123      100 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/tests/generators/invalid-conditions.clvm
--rw-r--r--   0     1001      123     1339 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/tests/generators/just-puzzle-announce.clvm
--rw-r--r--   0     1001      123   590571 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/tests/generators/many-create-coin.clvm
--rw-r--r--   0     1001      123      597 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/tests/generators/many-large-ints-negative.clvm
--rw-r--r--   0     1001      123      416 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/tests/generators/many-large-ints.clvm
--rw-r--r--   0     1001      123      500 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/tests/generators/max-height.clvm
--rw-r--r--   0     1001      123      349 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/tests/generators/multiple-reserve-fee.clvm
--rw-r--r--   0     1001      123      400 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/tests/generators/negative-reserve-fee.clvm
--rw-r--r--   0     1001      123      160 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/tests/generators/recursion-pairs.clvm
--rw-r--r--   0     1001      123      343 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/tests/generators/unknown-condition.clvm
--rwxr-xr-x   0     1001      123     3042 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/tests/run-programs.py
--rwxr-xr-x   0     1001      123     1569 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/tests/run.py
--rwxr-xr-x   0     1001      123     3789 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/tests/run_gen.py
--rwxr-xr-x   0     1001      123     3497 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/tests/test-generators.py
--rw-r--r--   0     1001      123    11060 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/tests/test_coin.py
--rw-r--r--   0     1001      123     5068 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/tests/test_run_puzzle.py
--rw-r--r--   0     1001      123    10725 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/tests/test_streamable.py
--rw-r--r--   0     1001      123     1050 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/chia/tests/test_tree_hash.py
--rw-r--r--   0        0        0      364 1970-01-01 00:00:00.000000 chia_rs-0.2.5/local_dependencies/clvm-utils/Cargo.toml
--rw-r--r--   0     1001      123      155 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/clvm-utils/README.md
--rw-r--r--   0     1001      123       36 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/clvm-utils/src/lib.rs
--rw-r--r--   0     1001      123     2918 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/clvm-utils/src/tree_hash.rs
--rw-r--r--   0     1001      123     6300 2023-03-16 22:58:13.000000 chia_rs-0.2.5/local_dependencies/clvm-utils/src/uncurry.rs
--rw-r--r--   0        0        0      890 1970-01-01 00:00:00.000000 chia_rs-0.2.5/Cargo.toml
--rw-r--r--   0     1001      123       77 2023-03-16 22:58:13.000000 chia_rs-0.2.5/README.md
--rw-r--r--   0     1001      123    68299 2023-03-16 22:58:13.000000 chia_rs-0.2.5/chia_rs.pyi
--rw-r--r--   0     1001      123     7396 2023-03-16 22:58:13.000000 chia_rs-0.2.5/generate_type_stubs.py
--rw-r--r--   0     1001      123        0 2023-03-16 22:58:13.000000 chia_rs-0.2.5/py.typed
--rw-r--r--   0     1001      123      112 2023-03-16 22:58:13.000000 chia_rs-0.2.5/pyproject.toml
--rw-r--r--   0     1001      123      615 2023-03-16 22:58:13.000000 chia_rs-0.2.5/src/adapt_response.rs
--rw-r--r--   0     1001      123     8865 2023-03-16 22:58:13.000000 chia_rs-0.2.5/src/api.rs
--rw-r--r--   0     1001      123      641 2023-03-16 22:58:13.000000 chia_rs-0.2.5/src/compression.rs
--rw-r--r--   0     1001      123      175 2023-03-16 22:58:13.000000 chia_rs-0.2.5/src/lib.rs
--rw-r--r--   0     1001      123     6946 2023-03-16 22:58:13.000000 chia_rs-0.2.5/src/run_generator.rs
--rw-r--r--   0     1001      123     2644 2023-03-16 22:58:13.000000 chia_rs-0.2.5/src/run_program.rs
--rw-r--r--   0     1001      123    14130 2023-03-16 22:59:34.000000 chia_rs-0.2.5/Cargo.lock
--rw-r--r--   0        0        0      483 1970-01-01 00:00:00.000000 chia_rs-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      781 1970-01-01 00:00:00.000000 chia_rs-0.2.6/local_dependencies/chia-protocol/Cargo.toml
+-rw-r--r--   0     1001      123      722 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia-protocol/src/bls.rs
+-rw-r--r--   0     1001      123     5474 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia-protocol/src/bytes.rs
+-rw-r--r--   0     1001      123     1386 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia-protocol/src/chia_error.rs
+-rw-r--r--   0     1001      123     4701 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia-protocol/src/chia_protocol.rs
+-rw-r--r--   0     1001      123      862 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia-protocol/src/classgroup.rs
+-rw-r--r--   0     1001      123     1809 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia-protocol/src/coin.rs
+-rw-r--r--   0     1001      123      556 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia-protocol/src/coin_spend.rs
+-rw-r--r--   0     1001      123      540 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia-protocol/src/coin_state.rs
+-rw-r--r--   0     1001      123      743 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia-protocol/src/end_of_sub_slot_bundle.rs
+-rw-r--r--   0     1001      123      871 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia-protocol/src/fee_estimate.rs
+-rw-r--r--   0     1001      123     2316 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia-protocol/src/foliage.rs
+-rw-r--r--   0     1001      123     3679 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia-protocol/src/from_json_dict.rs
+-rw-r--r--   0     1001      123     1497 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia-protocol/src/fullblock.rs
+-rw-r--r--   0     1001      123     1388 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia-protocol/src/header_block.rs
+-rw-r--r--   0     1001      123     1288 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia-protocol/src/lib.rs
+-rw-r--r--   0     1001      123      810 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia-protocol/src/message_struct.rs
+-rw-r--r--   0     1001      123      540 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia-protocol/src/pool_target.rs
+-rw-r--r--   0     1001      123     1624 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia-protocol/src/program.rs
+-rw-r--r--   0     1001      123      679 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia-protocol/src/proof_of_space.rs
+-rw-r--r--   0     1001      123     1527 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia-protocol/src/reward_chain_block.rs
+-rw-r--r--   0     1001      123     1788 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia-protocol/src/slots.rs
+-rw-r--r--   0     1001      123      569 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia-protocol/src/spend_bundle.rs
+-rw-r--r--   0     1001      123    20212 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia-protocol/src/streamable.rs
+-rw-r--r--   0     1001      123     2217 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia-protocol/src/to_json_dict.rs
+-rw-r--r--   0     1001      123      679 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia-protocol/src/vdf.rs
+-rw-r--r--   0     1001      123     4016 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia-protocol/src/wallet_protocol.rs
+-rw-r--r--   0     1001      123     1225 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia-protocol/src/weight_proof.rs
+-rw-r--r--   0        0        0      458 1970-01-01 00:00:00.000000 chia_rs-0.2.6/local_dependencies/chia_py_streamable_macro/Cargo.toml
+-rw-r--r--   0     1001      123     9330 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia_py_streamable_macro/src/lib.rs
+-rw-r--r--   0        0        0     1001 1970-01-01 00:00:00.000000 chia_rs-0.2.6/local_dependencies/chia/Cargo.toml
+-rw-r--r--   0     1001      123      224 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/.cargo/config
+-rw-r--r--   0     1001      123      290 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/.github/workflows/audit-check.yml
+-rw-r--r--   0     1001      123     3050 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/.github/workflows/benchmark.yml
+-rw-r--r--   0     1001      123     2843 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/.github/workflows/build-crate-and-npm.yml
+-rw-r--r--   0     1001      123    13503 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/.github/workflows/build-test.yml
+-rw-r--r--   0     1001      123       19 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/.gitignore
+-rw-r--r--   0     1001      123    11357 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/LICENSE
+-rw-r--r--   0     1001      123      192 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/README.md
+-rw-r--r--   0     1001      123      142 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/cl/README.md
+-rw-r--r--   0     1001      123     4603 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/cl/deserialize_w_backrefs.cl
+-rw-r--r--   0     1001      123     4474 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/docs/implementation-notes.md
+-rw-r--r--   0     1001      123      882 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/examples/README.md
+-rw-r--r--   0     1001      123    48843 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/examples/block-1519806.bin
+-rw-r--r--   0     1001      123      299 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/examples/dump.py
+-rw-r--r--   0     1001      123     1592 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/examples/streaming-patch.diff
+-rw-r--r--   0     1001      123       93 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/mypy.ini
+-rw-r--r--   0     1001      123      261 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/src/allocator.rs
+-rw-r--r--   0     1001      123     1817 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/src/compression/compressor.rs
+-rw-r--r--   0     1001      123      858 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/src/compression/deserialize_w_backrefs.bin
+-rw-r--r--   0     1001      123       20 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/src/compression/mod.rs
+-rw-r--r--   0     1001      123     3120 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/src/fuzzing_utils.rs
+-rw-r--r--   0     1001      123     3042 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/src/gen/coin_id.rs
+-rw-r--r--   0     1001      123     4493 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/src/gen/condition_sanitizers.rs
+-rw-r--r--   0     1001      123   129755 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/src/gen/conditions.rs
+-rw-r--r--   0     1001      123      972 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/src/gen/flags.rs
+-rw-r--r--   0     1001      123     6447 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/src/gen/get_puzzle_and_solution.rs
+-rw-r--r--   0     1001      123      221 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/src/gen/mod.rs
+-rw-r--r--   0     1001      123     7075 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/src/gen/opcodes.rs
+-rw-r--r--   0     1001      123     2305 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/src/gen/run_block_generator.rs
+-rw-r--r--   0     1001      123     2159 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/src/gen/run_puzzle.rs
+-rw-r--r--   0     1001      123     2916 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/src/gen/sanitize_int.rs
+-rw-r--r--   0     1001      123     5743 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/src/gen/validation_error.rs
+-rw-r--r--   0     1001      123     4972 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/src/generator_rom.rs
+-rw-r--r--   0     1001      123      136 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/src/lib.rs
+-rw-r--r--   0     1001      123    22862 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/src/merkle_set.rs
+-rwxr-xr-x   0     1001      123     8264 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/tests/generate-programs.py
+-rw-r--r--   0     1001      123     1143 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/tests/generators/assert-puzzle-announce-fail.clvm
+-rw-r--r--   0     1001      123    21116 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/tests/generators/block-834752.clvm
+-rw-r--r--   0     1001      123    25761 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/tests/generators/block-834752.hex
+-rw-r--r--   0     1001      123    99972 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/tests/generators/block-834760.clvm
+-rw-r--r--   0     1001      123    22001 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/tests/generators/block-834761.clvm
+-rw-r--r--   0     1001      123    59172 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/tests/generators/block-834765.clvm
+-rw-r--r--   0     1001      123   105717 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/tests/generators/block-834766.clvm
+-rw-r--r--   0     1001      123    83316 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/tests/generators/block-834768.clvm
+-rw-r--r--   0     1001      123      577 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/tests/generators/create-coin-different-amounts.clvm
+-rw-r--r--   0     1001      123      267 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/tests/generators/create-coin-hint-duplicate-outputs.clvm
+-rw-r--r--   0     1001      123      685 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/tests/generators/create-coin-hint.clvm
+-rw-r--r--   0     1001      123      699 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/tests/generators/create-coin-hint2.clvm
+-rw-r--r--   0     1001      123      456 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/tests/generators/deep-recursion-plus.clvm
+-rw-r--r--   0     1001      123      382 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/tests/generators/double-spend.clvm
+-rw-r--r--   0     1001      123      501 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/tests/generators/duplicate-coin-announce.clvm
+-rw-r--r--   0     1001      123      263 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/tests/generators/duplicate-create-coin.clvm
+-rw-r--r--   0     1001      123      448 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/tests/generators/duplicate-height-absolute-div.clvm
+-rw-r--r--   0     1001      123      429 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/tests/generators/duplicate-height-absolute-substr-tail.clvm
+-rw-r--r--   0     1001      123      422 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/tests/generators/duplicate-height-absolute-substr.clvm
+-rw-r--r--   0     1001      123      391 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/tests/generators/duplicate-height-absolute.clvm
+-rw-r--r--   0     1001      123      391 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/tests/generators/duplicate-height-relative.clvm
+-rw-r--r--   0     1001      123      196 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/tests/generators/duplicate-outputs.clvm
+-rw-r--r--   0     1001      123      391 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/tests/generators/duplicate-reserve-fee.clvm
+-rw-r--r--   0     1001      123      391 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/tests/generators/duplicate-seconds-absolute.clvm
+-rw-r--r--   0     1001      123      392 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/tests/generators/duplicate-seconds-relative.clvm
+-rw-r--r--   0     1001      123      380 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/tests/generators/height-absolute-ladder.clvm
+-rw-r--r--   0     1001      123      104 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/tests/generators/infinite-recursion1.clvm
+-rw-r--r--   0     1001      123       92 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/tests/generators/infinite-recursion2.clvm
+-rw-r--r--   0     1001      123     1458 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/tests/generators/infinite-recursion3.clvm
+-rw-r--r--   0     1001      123      160 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/tests/generators/infinite-recursion4.clvm
+-rw-r--r--   0     1001      123      100 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/tests/generators/invalid-conditions.clvm
+-rw-r--r--   0     1001      123     1339 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/tests/generators/just-puzzle-announce.clvm
+-rw-r--r--   0     1001      123   590571 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/tests/generators/many-create-coin.clvm
+-rw-r--r--   0     1001      123      597 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/tests/generators/many-large-ints-negative.clvm
+-rw-r--r--   0     1001      123      416 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/tests/generators/many-large-ints.clvm
+-rw-r--r--   0     1001      123      500 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/tests/generators/max-height.clvm
+-rw-r--r--   0     1001      123      349 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/tests/generators/multiple-reserve-fee.clvm
+-rw-r--r--   0     1001      123      400 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/tests/generators/negative-reserve-fee.clvm
+-rw-r--r--   0     1001      123      160 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/tests/generators/recursion-pairs.clvm
+-rw-r--r--   0     1001      123      343 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/tests/generators/unknown-condition.clvm
+-rwxr-xr-x   0     1001      123     3042 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/tests/run-programs.py
+-rwxr-xr-x   0     1001      123     1569 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/tests/run.py
+-rwxr-xr-x   0     1001      123     3789 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/tests/run_gen.py
+-rwxr-xr-x   0     1001      123     3497 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/tests/test-generators.py
+-rw-r--r--   0     1001      123    11060 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/tests/test_coin.py
+-rw-r--r--   0     1001      123     5068 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/tests/test_run_puzzle.py
+-rw-r--r--   0     1001      123    10725 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/tests/test_streamable.py
+-rw-r--r--   0     1001      123     1050 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia/tests/test_tree_hash.py
+-rw-r--r--   0        0        0      470 1970-01-01 00:00:00.000000 chia_rs-0.2.6/local_dependencies/chia_streamable_macro/Cargo.toml
+-rw-r--r--   0     1001      123     4715 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/chia_streamable_macro/src/lib.rs
+-rw-r--r--   0        0        0      364 1970-01-01 00:00:00.000000 chia_rs-0.2.6/local_dependencies/clvm-utils/Cargo.toml
+-rw-r--r--   0     1001      123      155 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/clvm-utils/README.md
+-rw-r--r--   0     1001      123       36 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/clvm-utils/src/lib.rs
+-rw-r--r--   0     1001      123     2918 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/clvm-utils/src/tree_hash.rs
+-rw-r--r--   0     1001      123     6300 2023-04-19 00:48:18.000000 chia_rs-0.2.6/local_dependencies/clvm-utils/src/uncurry.rs
+-rw-r--r--   0        0        0      890 1970-01-01 00:00:00.000000 chia_rs-0.2.6/Cargo.toml
+-rw-r--r--   0     1001      123       77 2023-04-19 00:48:18.000000 chia_rs-0.2.6/README.md
+-rw-r--r--   0     1001      123    68299 2023-04-19 00:48:18.000000 chia_rs-0.2.6/chia_rs.pyi
+-rw-r--r--   0     1001      123     7396 2023-04-19 00:48:18.000000 chia_rs-0.2.6/generate_type_stubs.py
+-rw-r--r--   0     1001      123        0 2023-04-19 00:48:18.000000 chia_rs-0.2.6/py.typed
+-rw-r--r--   0     1001      123      112 2023-04-19 00:48:18.000000 chia_rs-0.2.6/pyproject.toml
+-rw-r--r--   0     1001      123      615 2023-04-19 00:48:18.000000 chia_rs-0.2.6/src/adapt_response.rs
+-rw-r--r--   0     1001      123     8865 2023-04-19 00:48:18.000000 chia_rs-0.2.6/src/api.rs
+-rw-r--r--   0     1001      123      641 2023-04-19 00:48:18.000000 chia_rs-0.2.6/src/compression.rs
+-rw-r--r--   0     1001      123      175 2023-04-19 00:48:18.000000 chia_rs-0.2.6/src/lib.rs
+-rw-r--r--   0     1001      123     6946 2023-04-19 00:48:18.000000 chia_rs-0.2.6/src/run_generator.rs
+-rw-r--r--   0     1001      123     2644 2023-04-19 00:48:18.000000 chia_rs-0.2.6/src/run_program.rs
+-rw-r--r--   0     1001      123    14442 2023-04-19 00:48:53.000000 chia_rs-0.2.6/Cargo.lock
+-rw-r--r--   0        0        0      483 1970-01-01 00:00:00.000000 chia_rs-0.2.6/PKG-INFO
```

### Comparing `chia_rs-0.2.5/local_dependencies/chia_streamable_macro/src/lib.rs` & `chia_rs-0.2.6/local_dependencies/chia_streamable_macro/src/lib.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia_py_streamable_macro/src/lib.rs` & `chia_rs-0.2.6/local_dependencies/chia_py_streamable_macro/src/lib.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia-protocol/Cargo.toml` & `chia_rs-0.2.6/local_dependencies/chia-protocol/Cargo.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "chia-protocol"
-version = "0.2.5"
+version = "0.2.6"
 edition = "2021"
 license = "Apache-2.0"
 description = "Chia network protocol message types"
 authors = ["Arvid Norberg <arvid@chia.net>"]
 homepage = "https://github.com/Chia-Network/chia_rs/chia-protocol/"
 repository = "https://github.com/Chia-Network/chia_rs/chia-protocol/"
 
@@ -13,11 +13,11 @@
 
 [dependencies]
 pyo3 = { version = "=0.15.1", features = ["extension-module", "multiple-pymethods"], optional = true }
 sha2 = "=0.10.2"
 hex = "=0.4.3"
 chia_streamable_macro = { version = "=0.2.4", path = "../chia_streamable_macro" }
 chia_py_streamable_macro = { path = "../chia_py_streamable_macro", version = "=0.1.3", optional = true }
-clvmr = "=0.2.3"
+clvmr = "=0.2.4"
 
 [lib]
 crate-type = ["rlib"]
```

### Comparing `chia_rs-0.2.5/local_dependencies/chia-protocol/src/bls.rs` & `chia_rs-0.2.6/local_dependencies/chia-protocol/src/bls.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia-protocol/src/bytes.rs` & `chia_rs-0.2.6/local_dependencies/chia-protocol/src/bytes.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia-protocol/src/chia_error.rs` & `chia_rs-0.2.6/local_dependencies/chia-protocol/src/chia_error.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia-protocol/src/chia_protocol.rs` & `chia_rs-0.2.6/local_dependencies/chia-protocol/src/chia_protocol.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia-protocol/src/classgroup.rs` & `chia_rs-0.2.6/local_dependencies/chia-protocol/src/classgroup.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia-protocol/src/coin.rs` & `chia_rs-0.2.6/local_dependencies/chia-protocol/src/coin.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia-protocol/src/coin_spend.rs` & `chia_rs-0.2.6/local_dependencies/chia-protocol/src/coin_spend.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia-protocol/src/coin_state.rs` & `chia_rs-0.2.6/local_dependencies/chia-protocol/src/coin_state.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia-protocol/src/end_of_sub_slot_bundle.rs` & `chia_rs-0.2.6/local_dependencies/chia-protocol/src/end_of_sub_slot_bundle.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia-protocol/src/fee_estimate.rs` & `chia_rs-0.2.6/local_dependencies/chia-protocol/src/fee_estimate.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia-protocol/src/foliage.rs` & `chia_rs-0.2.6/local_dependencies/chia-protocol/src/foliage.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia-protocol/src/from_json_dict.rs` & `chia_rs-0.2.6/local_dependencies/chia-protocol/src/from_json_dict.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia-protocol/src/fullblock.rs` & `chia_rs-0.2.6/local_dependencies/chia-protocol/src/fullblock.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia-protocol/src/header_block.rs` & `chia_rs-0.2.6/local_dependencies/chia-protocol/src/header_block.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia-protocol/src/lib.rs` & `chia_rs-0.2.6/local_dependencies/chia-protocol/src/lib.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia-protocol/src/message_struct.rs` & `chia_rs-0.2.6/local_dependencies/chia-protocol/src/message_struct.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia-protocol/src/pool_target.rs` & `chia_rs-0.2.6/local_dependencies/chia-protocol/src/pool_target.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia-protocol/src/program.rs` & `chia_rs-0.2.6/local_dependencies/chia-protocol/src/program.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia-protocol/src/proof_of_space.rs` & `chia_rs-0.2.6/local_dependencies/chia-protocol/src/proof_of_space.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia-protocol/src/reward_chain_block.rs` & `chia_rs-0.2.6/local_dependencies/chia-protocol/src/reward_chain_block.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia-protocol/src/slots.rs` & `chia_rs-0.2.6/local_dependencies/chia-protocol/src/slots.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia-protocol/src/spend_bundle.rs` & `chia_rs-0.2.6/local_dependencies/chia-protocol/src/spend_bundle.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia-protocol/src/streamable.rs` & `chia_rs-0.2.6/local_dependencies/chia-protocol/src/streamable.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia-protocol/src/to_json_dict.rs` & `chia_rs-0.2.6/local_dependencies/chia-protocol/src/to_json_dict.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia-protocol/src/vdf.rs` & `chia_rs-0.2.6/local_dependencies/chia-protocol/src/vdf.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia-protocol/src/wallet_protocol.rs` & `chia_rs-0.2.6/local_dependencies/chia-protocol/src/wallet_protocol.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia-protocol/src/weight_proof.rs` & `chia_rs-0.2.6/local_dependencies/chia-protocol/src/weight_proof.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia/Cargo.toml` & `chia_rs-0.2.6/local_dependencies/chia/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,31 +2,31 @@
 # "cargo test" and "cargo bench"
 [workspace]
 members = ["wasm", "chia_streamable_macro", "chia-bls", "clvm-utils", "chia-protocol", "chia_py_streamable_macro", "chia-tools"]
 exclude = ["wheel"]
 
 [package]
 name = "chia"
-version = "0.2.5"
+version = "0.2.6"
 edition = "2021"
 license = "Apache-2.0"
 description = "Utility functions and types used by the Chia blockchain full node"
 authors = ["Richard Kiss <him@richardkiss.com>", "Arvid Norberg <arvid@chia.net>"]
 homepage = "https://github.com/Chia-Network/chia_rs/"
 repository = "https://github.com/Chia-Network/chia_rs/"
 
 [features]
 py-bindings = ["dep:pyo3"]
 
 [dependencies]
-clvmr = "=0.2.3"
+clvmr = "=0.2.4"
 hex = "=0.4.3"
 pyo3 = { version = "=0.15.1", features = ["extension-module"], optional = true }
-clvm-utils = { version = "=0.2.5", path = "../clvm-utils" }
-chia-protocol = { version = "=0.2.5", path = "../chia-protocol" }
+clvm-utils = { version = "=0.2.6", path = "../clvm-utils" }
+chia-protocol = { version = "=0.2.6", path = "../chia-protocol" }
 
 [lib]
 name = "chia"
 crate-type = ["rlib"]
 
 [profile.release]
 lto = true
```

### Comparing `chia_rs-0.2.5/local_dependencies/chia/.github/workflows/benchmark.yml` & `chia_rs-0.2.6/local_dependencies/chia/.github/workflows/benchmark.yml`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia/.github/workflows/build-crate-and-npm.yml` & `chia_rs-0.2.6/local_dependencies/chia/.github/workflows/build-crate-and-npm.yml`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia/.github/workflows/build-test.yml` & `chia_rs-0.2.6/local_dependencies/chia/.github/workflows/build-test.yml`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia/LICENSE` & `chia_rs-0.2.6/local_dependencies/chia/LICENSE`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia/cl/deserialize_w_backrefs.cl` & `chia_rs-0.2.6/local_dependencies/chia/cl/deserialize_w_backrefs.cl`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia/docs/implementation-notes.md` & `chia_rs-0.2.6/local_dependencies/chia/docs/implementation-notes.md`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia/examples/README.md` & `chia_rs-0.2.6/local_dependencies/chia/examples/README.md`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia/examples/block-1519806.bin` & `chia_rs-0.2.6/local_dependencies/chia/examples/block-1519806.bin`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia/examples/streaming-patch.diff` & `chia_rs-0.2.6/local_dependencies/chia/examples/streaming-patch.diff`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia/src/compression/compressor.rs` & `chia_rs-0.2.6/local_dependencies/chia/src/compression/compressor.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia/src/compression/deserialize_w_backrefs.bin` & `chia_rs-0.2.6/local_dependencies/chia/src/compression/deserialize_w_backrefs.bin`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia/src/fuzzing_utils.rs` & `chia_rs-0.2.6/local_dependencies/chia/src/fuzzing_utils.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia/src/gen/coin_id.rs` & `chia_rs-0.2.6/local_dependencies/chia/src/gen/coin_id.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia/src/gen/condition_sanitizers.rs` & `chia_rs-0.2.6/local_dependencies/chia/src/gen/condition_sanitizers.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia/src/gen/conditions.rs` & `chia_rs-0.2.6/local_dependencies/chia/src/gen/conditions.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia/src/gen/flags.rs` & `chia_rs-0.2.6/local_dependencies/chia/src/gen/flags.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia/src/gen/get_puzzle_and_solution.rs` & `chia_rs-0.2.6/local_dependencies/chia/src/gen/get_puzzle_and_solution.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia/src/gen/opcodes.rs` & `chia_rs-0.2.6/local_dependencies/chia/src/gen/opcodes.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia/src/gen/run_block_generator.rs` & `chia_rs-0.2.6/local_dependencies/chia/src/gen/run_block_generator.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia/src/gen/run_puzzle.rs` & `chia_rs-0.2.6/local_dependencies/chia/src/gen/run_puzzle.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia/src/gen/sanitize_int.rs` & `chia_rs-0.2.6/local_dependencies/chia/src/gen/sanitize_int.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia/src/gen/validation_error.rs` & `chia_rs-0.2.6/local_dependencies/chia/src/gen/validation_error.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia/src/generator_rom.rs` & `chia_rs-0.2.6/local_dependencies/chia/src/generator_rom.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia/src/merkle_set.rs` & `chia_rs-0.2.6/local_dependencies/chia/src/merkle_set.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia/tests/generate-programs.py` & `chia_rs-0.2.6/local_dependencies/chia/tests/generate-programs.py`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia/tests/generators/assert-puzzle-announce-fail.clvm` & `chia_rs-0.2.6/local_dependencies/chia/tests/generators/assert-puzzle-announce-fail.clvm`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia/tests/generators/block-834752.clvm` & `chia_rs-0.2.6/local_dependencies/chia/tests/generators/block-834752.clvm`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia/tests/generators/block-834752.hex` & `chia_rs-0.2.6/local_dependencies/chia/tests/generators/block-834752.hex`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia/tests/generators/block-834760.clvm` & `chia_rs-0.2.6/local_dependencies/chia/tests/generators/block-834760.clvm`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia/tests/generators/block-834761.clvm` & `chia_rs-0.2.6/local_dependencies/chia/tests/generators/block-834761.clvm`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia/tests/generators/block-834765.clvm` & `chia_rs-0.2.6/local_dependencies/chia/tests/generators/block-834765.clvm`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia/tests/generators/block-834766.clvm` & `chia_rs-0.2.6/local_dependencies/chia/tests/generators/block-834766.clvm`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia/tests/generators/block-834768.clvm` & `chia_rs-0.2.6/local_dependencies/chia/tests/generators/block-834768.clvm`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia/tests/generators/create-coin-different-amounts.clvm` & `chia_rs-0.2.6/local_dependencies/chia/tests/generators/create-coin-different-amounts.clvm`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia/tests/generators/create-coin-hint.clvm` & `chia_rs-0.2.6/local_dependencies/chia/tests/generators/create-coin-hint.clvm`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia/tests/generators/create-coin-hint2.clvm` & `chia_rs-0.2.6/local_dependencies/chia/tests/generators/create-coin-hint2.clvm`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia/tests/generators/infinite-recursion3.clvm` & `chia_rs-0.2.6/local_dependencies/chia/tests/generators/infinite-recursion3.clvm`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia/tests/generators/just-puzzle-announce.clvm` & `chia_rs-0.2.6/local_dependencies/chia/tests/generators/just-puzzle-announce.clvm`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia/tests/generators/many-create-coin.clvm` & `chia_rs-0.2.6/local_dependencies/chia/tests/generators/many-create-coin.clvm`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia/tests/generators/many-large-ints-negative.clvm` & `chia_rs-0.2.6/local_dependencies/chia/tests/generators/many-large-ints-negative.clvm`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia/tests/run-programs.py` & `chia_rs-0.2.6/local_dependencies/chia/tests/run-programs.py`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia/tests/run.py` & `chia_rs-0.2.6/local_dependencies/chia/tests/run.py`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia/tests/run_gen.py` & `chia_rs-0.2.6/local_dependencies/chia/tests/run_gen.py`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia/tests/test-generators.py` & `chia_rs-0.2.6/local_dependencies/chia/tests/test-generators.py`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia/tests/test_coin.py` & `chia_rs-0.2.6/local_dependencies/chia/tests/test_coin.py`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia/tests/test_run_puzzle.py` & `chia_rs-0.2.6/local_dependencies/chia/tests/test_run_puzzle.py`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia/tests/test_streamable.py` & `chia_rs-0.2.6/local_dependencies/chia/tests/test_streamable.py`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/chia/tests/test_tree_hash.py` & `chia_rs-0.2.6/local_dependencies/chia/tests/test_tree_hash.py`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/clvm-utils/src/tree_hash.rs` & `chia_rs-0.2.6/local_dependencies/clvm-utils/src/tree_hash.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/local_dependencies/clvm-utils/src/uncurry.rs` & `chia_rs-0.2.6/local_dependencies/clvm-utils/src/uncurry.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/chia_rs.pyi` & `chia_rs-0.2.6/chia_rs.pyi`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/generate_type_stubs.py` & `chia_rs-0.2.6/generate_type_stubs.py`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/src/adapt_response.rs` & `chia_rs-0.2.6/src/adapt_response.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/src/api.rs` & `chia_rs-0.2.6/src/api.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/src/compression.rs` & `chia_rs-0.2.6/src/compression.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/src/run_generator.rs` & `chia_rs-0.2.6/src/run_generator.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/src/run_program.rs` & `chia_rs-0.2.6/src/run_program.rs`

 * *Files identical despite different names*

### Comparing `chia_rs-0.2.5/Cargo.lock` & `chia_rs-0.2.6/Cargo.lock`

 * *Files 10% similar despite different names*

```diff
@@ -52,46 +52,46 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chia"
-version = "0.2.5"
+version = "0.2.6"
 dependencies = [
  "chia-protocol",
  "clvm-utils",
  "clvmr",
  "hex",
  "pyo3",
 ]
 
 [[package]]
 name = "chia-protocol"
-version = "0.2.5"
+version = "0.2.6"
 dependencies = [
  "chia_py_streamable_macro",
  "chia_streamable_macro",
  "clvmr",
  "hex",
  "pyo3",
  "sha2",
 ]
 
 [[package]]
 name = "chia_py_streamable_macro"
 version = "0.1.3"
 dependencies = [
  "quote",
- "syn",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "chia_rs"
-version = "0.2.5"
+version = "0.2.6"
 dependencies = [
  "chia",
  "chia-protocol",
  "chia_py_streamable_macro",
  "chia_streamable_macro",
  "clvmr",
  "hex",
@@ -99,44 +99,44 @@
 ]
 
 [[package]]
 name = "chia_streamable_macro"
 version = "0.2.4"
 dependencies = [
  "quote",
- "syn",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "clvm-utils"
-version = "0.2.5"
+version = "0.2.6"
 dependencies = [
  "clvmr",
 ]
 
 [[package]]
 name = "clvmr"
-version = "0.2.3"
+version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0a2c6a0771a4efb01e3a492138e8d87e2d58f3740fcd0be020c7e597c1498387"
+checksum = "93dfa322573fe20cb086a246f5d5f064d2b3c1cb7ea5b6b7687a0cbddac20bd7"
 dependencies = [
  "bls12_381",
  "hex",
  "lazy_static",
  "num-bigint",
  "num-integer",
  "num-traits",
  "sha2",
 ]
 
 [[package]]
 name = "cpufeatures"
-version = "0.2.5"
+version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "28d997bd5e24a5928dd43e46dc529867e207907fe0b239c3477d924f7f2ca320"
+checksum = "280a9f2d8b3a38871a3c8a46fb80db65e5e5ed97da80c4d08bf27fb63e35e181"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "crypto-common"
 version = "0.1.6"
@@ -150,15 +150,15 @@
 [[package]]
 name = "ctor"
 version = "0.1.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6d2301688392eb071b0bf1a37be05c469d3cc4dbbd95df672fe28ab021e6a096"
 dependencies = [
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "digest"
 version = "0.10.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8168378f4e5023e7218c89c891c0fd8ecdb5e5e4f18cb78f38cf245dd021e76f"
@@ -182,31 +182,31 @@
 name = "funty"
 version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e6d5a32815ae3f33302d95fdcb2ce17862f8c65363dcfd29360480ba1001fc9c"
 
 [[package]]
 name = "generic-array"
-version = "0.14.6"
+version = "0.14.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bff49e947297f3312447abdca79f45f4738097cc82b06e72054d2223f601f1b9"
+checksum = "85649ca51fd72272d7821adaf274ad91c288277713d9c18820d8499a7ff69e9a"
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
 name = "ghost"
-version = "0.1.8"
+version = "0.1.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "69e0cd8a998937e25c6ba7cc276b96ec5cc3f4dc4ab5de9ede4fb152bdd5c5eb"
+checksum = "e77ac7b51b8e6313251737fcef4b1c01a2ea102bde68415b62c0ee9268fec357"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "group"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5dfbfb3a6cfbd390d5c9564ab283a0349b9b9fcd46a706c1eb10e0db70bfbac7"
@@ -237,15 +237,15 @@
 version = "0.3.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ce046d161f000fffde5f432a0d034d0341dc152643b2598ed5bfce44c4f3a8f0"
 dependencies = [
  "proc-macro-hack",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
  "unindent",
 ]
 
 [[package]]
 name = "instant"
 version = "0.1.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -269,28 +269,28 @@
 name = "inventory-impl"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7e41b53715c6f0c4be49510bb82dee2c1e51c8586d885abe65396e82ed518548"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.140"
+version = "0.2.141"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "99227334921fae1a979cf0bfdfcc6b3e5ce376ef57e16fb6fb3ea2ed6095f80c"
+checksum = "3304a64d199bb964be99741b7a14d26972741915b3649639149b2479bb46f4b5"
 
 [[package]]
 name = "lock_api"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
 dependencies = [
@@ -391,17 +391,17 @@
 name = "proc-macro-hack"
 version = "0.5.20+deprecated"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc375e1527247fe1a97d8b7156678dfe7c1af2fc075c9a4db3690ecd2a148068"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.52"
+version = "1.0.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1d0e1ae9e836cc3beddd63db0df682593d7e2d3d891ae8c9083d2113e1744224"
+checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.15.1"
@@ -432,27 +432,27 @@
 name = "pyo3-macros"
 version = "0.15.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "67701eb32b1f9a9722b4bc54b548ff9d7ebfded011c12daece7b9063be1fd755"
 dependencies = [
  "pyo3-macros-backend",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
 version = "0.15.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f44f09e825ee49a105f2c7b23ebee50886a9aee0746f4dd5a704138a64b0218a"
 dependencies = [
  "proc-macro2",
  "pyo3-build-config",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
 version = "1.0.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
@@ -518,14 +518,25 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
+name = "syn"
+version = "2.0.15"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a34fcf3e8b60f57e6a14301a2e916d323af98b0ea63c599441eec8558660c822"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "unicode-ident",
+]
+
+[[package]]
 name = "tap"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "55937e1799185b12863d447f42597ed69d9928686b8d88a1df17376a097d8369"
 
 [[package]]
 name = "typenum"
```

