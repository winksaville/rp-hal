# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.2.0] - 2024-09-25

### Changed

- First version

## v0.3.0 (2024-11-03)

### New Features

 - <csr-id-91552901849792143400e9fc167a0255574250d1/> Document the aliases in README.me
   Also, tweak the aliases and add dev and release modes with shorter names.
 - <csr-id-7554d41e008fe1f738cf3bc6cfdbdd5fe371f896/> Make it easier to specify target architecture
       Create aliases build-arm run-arm build-riscv and run-riscv in
       .cargo/config.toml. With these defined you can now use the alias which
       will be converted to the full target name:
   
         cargo build-arm   -> cargo build --target thumbv8m.main-none-eabihf
         cargo run-arm     -> cargo run --target thumbv8m.main-none-eabihf
         cargo build-riscv -> cargo build --target riscv32imac-unknown-none-elf
         cargo run-risv    -> cargo run --target riscv32imac-unknown-none-elf
   
       Append --release parameter to do release builds and runs. For example:
   
         cargo run-riscv --release ->
                cargo run --target riscv32imac-unknown-none-elf --release
 - <csr-id-75dd2ebde77cf4148bc620ab6a9c4f123c7ed44b/> add support for PIO `in_count`

### Bug Fixes

 - <csr-id-416cdc7dc3c17de34ec0828ef6882d238d2b929a/> Apply review suggestions from theJPster
 - <csr-id-ab443408a8a7111c60ea285f939979a4d6f60a98/> More clean up
 - <csr-id-c61b023670c7dd3a07feeb0328e44a98cb9d83a2/> Adding reviewers suggestions

### Other

 - <csr-id-b984c6b2ef1da159f6a69c1ecb3ec91a9c05e9ae/> Update rp235x-hal to use cargo-release
   Update CHANGELOG.md it so it includes [0.2.0] release information.
   Add release.toml
 - <csr-id-982dbb1e1e2a01d3fa927ae509dffe1255a4e756/> port `set_format` changes to rp235x
 - <csr-id-0e945d50d625487dfbb604778af85e84db4c3f8a/> remove undesired parameter to `set_format`

### Commit Statistics

<csr-read-only-do-not-edit/>

 - 30 commits contributed to the release.
 - 39 days passed between releases.
 - 9 commits were understood as [conventional](https://www.conventionalcommits.org).
 - 0 issues like '(#ID)' were seen in commit messages

### Commit Details

<csr-read-only-do-not-edit/>

<details><summary>view details</summary>

 * **Uncategorized**
    - Update rp235x-hal to use cargo-release ([`b984c6b`](https://github.com/winksaville/rp-hal/commit/b984c6b2ef1da159f6a69c1ecb3ec91a9c05e9ae))
    - Merge pull request #869 from winksaville/Make-it-easier-to-specify-target-architecture ([`e87e2ac`](https://github.com/winksaville/rp-hal/commit/e87e2acc233a9e3b54a9287dc2a7285db1969cad))
    - Update rp235x-hal-examples/README.md ([`8ebc0ab`](https://github.com/winksaville/rp-hal/commit/8ebc0ab5825948280a62832292ff04264f1abe78))
    - Apply suggestions from code review ([`7fc0d6a`](https://github.com/winksaville/rp-hal/commit/7fc0d6a26ddb2de1cbeac58df90f2071a23ad0d3))
    - Update rp235x-hal-examples/README.md ([`033e5aa`](https://github.com/winksaville/rp-hal/commit/033e5aa5ad1a4e9e14cc6c3d732072f90615f5c6))
    - Apply review suggestions from theJPster ([`416cdc7`](https://github.com/winksaville/rp-hal/commit/416cdc7dc3c17de34ec0828ef6882d238d2b929a))
    - More clean up ([`ab44340`](https://github.com/winksaville/rp-hal/commit/ab443408a8a7111c60ea285f939979a4d6f60a98))
    - Adding reviewers suggestions ([`c61b023`](https://github.com/winksaville/rp-hal/commit/c61b023670c7dd3a07feeb0328e44a98cb9d83a2))
    - Document the aliases in README.me ([`9155290`](https://github.com/winksaville/rp-hal/commit/91552901849792143400e9fc167a0255574250d1))
    - Merge pull request #868 from allexoll/main ([`96ba900`](https://github.com/winksaville/rp-hal/commit/96ba900d26e61d940066dbeffc4b9b28252ad2d3))
    - Make it easier to specify target architecture ([`7554d41`](https://github.com/winksaville/rp-hal/commit/7554d41e008fe1f738cf3bc6cfdbdd5fe371f896))
    - Add support for PIO `in_count` ([`75dd2eb`](https://github.com/winksaville/rp-hal/commit/75dd2ebde77cf4148bc620ab6a9c4f123c7ed44b))
    - Merge pull request #866 from jannic/port-861-to-rp235x ([`247dce8`](https://github.com/winksaville/rp-hal/commit/247dce8c68d1be46c22ccd01f812252c908cc13a))
    - Implement Debug support for the GPIO structures (RP235x) ([`343f63f`](https://github.com/winksaville/rp-hal/commit/343f63f5e364fffdb751ba7e3e637405c40dd56d))
    - Implement Debug support for the GPIO structures ([`1bce4c9`](https://github.com/winksaville/rp-hal/commit/1bce4c9f3fdf6286b64cb258ab1d56db6f945cfe))
    - Merge pull request #865 from jannic/fix-beta-clippy ([`379530d`](https://github.com/winksaville/rp-hal/commit/379530d8b402463c1b6ec7da1c80912b79563796))
    - Copy changes from rp2040-hal-examples to rp235x-hal-examples ([`0d79844`](https://github.com/winksaville/rp-hal/commit/0d7984478cb75604e4fabc9df099bd62953cc7b0))
    - Fix several clippy warnings in examples ([`29aa62f`](https://github.com/winksaville/rp-hal/commit/29aa62f4e74e311e0372aaa585524230045c9ae6))
    - Suppress some clippy warnings in examples ([`5ad3adc`](https://github.com/winksaville/rp-hal/commit/5ad3adc79a36b4c9cb855507d28ca545bf30ab12))
    - Fix clippy warnings reported by rust beta ([`b89005b`](https://github.com/winksaville/rp-hal/commit/b89005b07a55f68a47359f03f9c3098410422347))
    - Merge pull request #862 from jannic/update-critical-section ([`00785b0`](https://github.com/winksaville/rp-hal/commit/00785b035b255c4a9d53bcd0610a8b1320caa1ce))
    - Merge pull request #863 from jannic/silence-warning-rust-1.82.0 ([`87d5124`](https://github.com/winksaville/rp-hal/commit/87d5124eb9860fdca35e04b435e05080fc5dc381))
    - Fix warning with rust 1.82.0 ([`b871f02`](https://github.com/winksaville/rp-hal/commit/b871f027a42fe035f8b44ceb521682ad15f2e228))
    - Merge pull request #860 from jannic/move-spi-set-format-to-any-state ([`ca4d23a`](https://github.com/winksaville/rp-hal/commit/ca4d23a149a7aee1f5b6da0d2e7fe4936d5cb561))
    - Update critical-section dependency to version 1.2.0 ([`445c002`](https://github.com/winksaville/rp-hal/commit/445c00266fe3f6470c03917c8226af755088f87f))
    - Port `set_format` changes to rp235x ([`982dbb1`](https://github.com/winksaville/rp-hal/commit/982dbb1e1e2a01d3fa927ae509dffe1255a4e756))
    - Remove undesired parameter to `set_format` ([`0e945d5`](https://github.com/winksaville/rp-hal/commit/0e945d50d625487dfbb604778af85e84db4c3f8a))
    - Merge pull request #857 from jannic/test-with-picotool ([`63af864`](https://github.com/winksaville/rp-hal/commit/63af8640a666ad329a0ddb1b8501a75d2ff61e3b))
    - Improve formatting of CI scripts ([`eb14a75`](https://github.com/winksaville/rp-hal/commit/eb14a75a5ef08030b1779febc49256a03ae93d70))
    - Run picotool step in github action ([`3f76f3e`](https://github.com/winksaville/rp-hal/commit/3f76f3e971a221bbe8ea5ce6ce38e853fa8a5759))
</details>

## v0.2.0 (2024-09-25)

### New Features

 - <csr-id-b83091377ffc7b671c19dcefc1d9257e4c52910e/> add support for aborting DMA transfers

### Other

 - <csr-id-01b9772501eadc21f694349ad3c9018c0576ee38/> fix typo in comment in rom_funcs
 - <csr-id-879d831e8800739f7bb3d1547d09bb8f28dbb2eb/> Fix alloc description
   Both examples had a typo in the description. That's now fixed.
 - <csr-id-95e0529b624dce5ca60d71cb5d6e4020a1c48e85/> Fix watchdog example comments.
   Both examples had a typo in the comments.
 - <csr-id-270a1dbb777c37d5a5ee06083b6627d14aa5990d/> Fix gpio_in_out description
   Both examples had a copy-pasta description. That's now fixed.
 - <csr-id-6ed9f06f1cbc33f07eb16b7c79ae40225f354c42/> More notes in the block-loop example.
 - <csr-id-aa7b66a731cb58484f75d82512f76413759ad832/> Formatting
 - <csr-id-b41c5a7e56c4d31e16dc3ff43a802bb007d1e0bb/> Mention the right board.
   Of course changing the board name caused every comment to re-wrap.
 - <csr-id-2173130b2ca1636d75347602fc852b60a62e9e8a/> More datasheet fixes.
 - <csr-id-17296c75df1a9d245c0d82ac2d97a2215ce27234/> switch to using picotool
   elf2uf2-rs doesn't work on RP2350. See https://github.com/JoNil/elf2uf2-rs/pull/33
 - <csr-id-86b4e69306a26630483e455e50f5c97bcffa88e6/> datasheet link clean-ups
   Also remove references to RP2040 that I missed.
 - <csr-id-f8016112933d1d746baa539f27e8f4363ed5804d/> move set_format to all states
   There are other drivers in the wild (uboot, zephyr) that set the format
   without disabling the peripheral, so we’ll assume it is fine to do so.
 - <csr-id-549ddbf190c2a8f362886409eb10784db1e1e0bc/> add `PinGroup::set_u32` to allow setting each pin to a different state
   * gpio: add `PinGroup::set_u32` to allow setting each pin to a different state
   
   * Add on-target-test for pin groups
   
   ---------
 - <csr-id-366d1496c771f1fc395be07572ab77607a00c955/> updates necessary because of rp2040-pac update
 - <csr-id-e9171381b67795ea559d451b61eaf3bc61c911c8/> update
 - <csr-id-8603abd0f4578eef2579654949e076bf49e6fe5d/> update
 - <csr-id-88aedf53a45d4b432c8318e26aba73a28c6c20fa/> updates
 - <csr-id-684a31206fa7f41bb3b6329414bf6f9bc4aa70ff/> Updates necessary because of rp2040-pac update
 - <csr-id-65309ff742e03ae84a1ae31ecb9b135d06cbe7b1/> add patch section to use updated rp2040-pac
 - <csr-id-bb7a98e3af8d9ca661b3f9be0375355a55f91cee/> add `categories` & `keywords`
   this makes it easier to find the crate, esp. when filtering by
   category.
   
   note that this will only become visible on crates.io once a new release
   has been published.
 - <csr-id-edc34435ebd816742e9d268961de87fba8277c4c/> i2c async: simplify transaction_iter
 - <csr-id-c99bf2abd5799bb7fd54af5e6a2d8a1a17864781/> Missed documentation update in copy/pase
 - <csr-id-821909ae812ece13c2f7c0deafdc0a4a5923b4e3/> Add getters to the various pad overrides (not type tracked)
 - <csr-id-4c72824859b6b2b229a1a3409132b26887619c0d/> reduce the number of spurious irq
 - <csr-id-6ad3d1e71ad1eba163cdb62fd3f08d26495b72f9/> Implement i2c-write-iter traits
 - <csr-id-7a47574795504a42ba2892ffa883338337ccaae5/> implement embedded-hal-async with tests
   Also adds "-Tdefmt.x" to .cargo/config.
   This required for i2c async examples & on-target-tests.
   Note this does not affect downstream dependents.
 - <csr-id-7d1bd63e57dc8f1e1a78797c0a5875b19391f75f/> add on-target-tests & fix discovered issues
 - <csr-id-4480c1d6f8fb13c1bf1aff69be28012c11e6ec1c/> :spi::MODE_0 -> embedded_hal::spi::MODE_0
 - <csr-id-04ce6ab5dbce496f1696fc22096275cc06f3a2c9/> Set TOP to 0xfffe by default and fix get_max_duty
   A TOP value of 0xffff is incompatible with true 100% duty cycle.
   Therefore, the default TOP value is reduced to 0xfffe, and a warning
   regarding the 0xffff value is added the documentation of `set_top`.
   
   The value returned by get_max_duty is corrected to be TOP + 1, if
   possible.
 - <csr-id-70ea42c4c6581219f3c5bb75ef906d6d2879f9f3/> Wait for CS.READY before draining fifo
 - <csr-id-01292212779342c860163a9a7e6d6481c828e1ad/> drain remaining values from FIFO, to prevent interrupts
 - <csr-id-63c761d0b58b3150c1533aa31a343a3f8c429694/> free-running mode experiments
 - <csr-id-79fac385f47878e98343868c763b0b599958ffed/> Fix undefined behaviour in multicore
   See these embassy PR for more explanation:
   - https://github.com/embassy-rs/embassy/pull/1459
   - https://github.com/embassy-rs/embassy/pull/1460
 - <csr-id-3e14a73fb4fca6a19c9ff18cb3d6d803403b487a/> Update comments & doc.
 - <csr-id-5a2ae8e7a2ffd01e0325dbfa7033b9d12237688b/> example application name
 - <csr-id-dfc790b207eb9a10a3f75e3522d0a90b7ef50891/> First frame is getting lost on a USB-CDC device.
   **Issue**
   
   While using `usb_device` and `usbd_serial` crates with `rp2040_hal`, the first frame from the host device is always getting lost. Consecutive frames work just fine.
   
   **Root Cause**
   The `LENGTH_0` region of the `EP_BUFFER_CONTROL` register is always reset (0) while waiting for the first frame. After the first frame failure, the poll operation implicitly sets it  to the necessary value (`max_packet_size`) and this clears the problem for the rest of the app execution life time.
   
   The main problem is while resetting and readjustment of the bits needs a step by step operation to avoid potential issues. While doing that and setting `AVAILABLE` bit, the wrong method had been chosen and was invalidating previous changes. Hence the `LENGTH_0` param is reset, too.
   
   **Proposed Solution**
   Instead of direct register `write` operation I've used `modify` to keep current bits in the register.
 - <csr-id-119534d2dae9d286a6f3eb0f52e253777f074d89/> Read ints rather than sie_status in poll
   If the latency is too high, there is a risk that the status reverts to a
   previous state while keeping the interrupt flag up.
   This fixes that by relying on ints instead of sie_status to process the
   events.
 - <csr-id-1b72a48870a49ecb66dff91b6053086ee94d11ec/> add docs.rs metadata
 - <csr-id-322bba2cc0f5e1fbc1698a85c96ff2d02db03f98/> Move interrupt related (en|dis)abling/forcing methods to the statemachine
   * pio: Move interrupt related (en|dis)abling/forcing methods to the statemachine
   
   The SM knows its id using the type system so there's no need for checking it.
   This commit also adds a `PioIRQ` enum to select the output IRQ.
   
   * Move the interrupt control to Rx & Tx and make all accesses to inte atomic
   * Adjust the ergonomics of IRQ handling.
   * Elide lifetimes where they can be (clippy's advice)
 - <csr-id-42fc266e67df78286a49cf8370c1f3fc6d9d33d0/> Mark Timer & Alarm* Send and Sync
 - <csr-id-993487443a9f002094bcd10b71f2f1fb6b6478d1/> clarify usage of boot2 section
 - <csr-id-5ce10ff94e1f019db3a1f8beb30ba21ec0ed14a4/> Use a fixed type in Alarm::schedule
 - <csr-id-6d75cd82912a486151f4f1b057ee5e60e0737e98/> Use the dedicated write_bitmask_* functions
 - <csr-id-f30df4a0c70d2939e7cf59cfd58882f1a4b60ee3/> Fix the link under the logo in rp2040-hal's readme
 - <csr-id-fea35b48bbfae75812dc7ab0ee78a70ffbc42985/> fix clocks extended usage xosc order
 - <csr-id-7840d0f8333d7a9a6dd0f07389d1d73c11caf97b/> Fix unexpected restart on repeated read.
 - <csr-id-f60828c9a4645414c916852ce3b877df1a317803/> Unmask rustc/ld warnings, remove deprecated '--all'
 - <csr-id-c02984b422d3cc12e14a3e17373f7bb3b57e5e58/> Remove mention of boot select button
   The boot selector pin is attached to SPI_SS and not easily read (an
   example
   https://github.com/raspberrypi/pico-examples/blob/master/picoboard/button/button.c),
   since the code reading needs to reside in sram.
   
   Simply fix the documentation
 - <csr-id-de536001995c07f9abf8026a72ed140aa0f08df1/> Handle errors of serial.write()
 - <csr-id-c7c5fb00d8b97d6fdcdaf66d67d5e0d85e9e580c/> Fix unsound Send clippy warning
 - <csr-id-233f7c947514b6b96ff8a146c2ddac8ac16ce510/> Add option --locked to cargo install elf2uf2-rs
   Without the --locked option, cargo currently tries to compile it using
   clap v3.0.0-beta.5, which fails:
   
   ```
   [...]
      Compiling clap v3.0.0-beta.5
      Compiling elf2uf2-rs v1.3.5
   error[E0432]: unresolved import `clap::Clap`
    -->
   /home/jan/.cargo/registry/src/github.com-1ecc6299db9ec823/elf2uf2-rs-1.3.5/src/main.rs:3:5
     |
   3 | use clap::Clap;
     |     ^^^^^^^^^^ no `Clap` in the root
   [...]
   ```
   
   With --locked, it uses clap v3.0.0-beta.4, which works.
 - <csr-id-c8bb2e43c792dd3975a255d7eba479547411aec6/> support zero post-divide
   This allows you to use a 62.5 MHz SPI baud rate assuming the default 125
   MHz peripheral clock. It would previously crash due to a division by
   zero.
 - <csr-id-4db944ad4e1096202f673cd85ddd3e6bcfa0f662/> Fix clippy warnings and examples in doc comments.
 - <csr-id-2fc42e07f235e42cb589bfb72c492013e5e54206/> Rename read_rx/write_tx to read/write.
 - <csr-id-207f5aebdbca7fe77823281cd5d8ac01f8f9badf/> Split RX and TX FIFO functions into different types.
   We need separate types for any blocking or DMA operations - otherwise, it
   would not be possible to perform both RX and TX transfers at the same time.
 - <csr-id-dbe7f48699a0fcc34217f64ffbbb20395ff363d8/> Identify state machines via generic parameters.
   Eventually, the read and write FIFOs need to be split into separate
   objects for DMA. To be able to safely rejoin them only when they belong to
   the same state machine, the state machine index needs to be encoded into
   the type.
 - <csr-id-64fa8441d8f2db125939c8bdce05973a0756042c/> Fix bugs spotted in the review.
 - <csr-id-684f4838590bb5ff809ded117f34364d7c65588e/> Improve documentation and add an example that uses pio_proc::pio!().
 - <csr-id-515eac5553e8a06908a73a37e24ec576b26969f5/> Differentiate between uninitialized/stopped/running state machines.
   Some operations must only be performed in a specific state. For example,
   pin directions must not be changed while the state machine is running, as
   the operation modifies PINCTRL. The new API makes wrong usage a lot harder.
   
   Also, the code now supports uninitializing state machines to free
   instruction space or to select a different function.
 - <csr-id-4d97d9fe75e6627d60ef8855832e4713bbae4c61/> Enable code sharing between SMs via objects for installed programs.
   Multiple state machines may want to execute the same program (e.g., two
   state machines are used to implement two I2C buses), in which code sharing
   saves space.
 - <csr-id-959f714fb95b8c585e5d5b539b820d0291178c5e/> Fix marking used instruction space.
 - <csr-id-2ff9ae156fcd437a3f087917ee699ec8de8646db/> Fix some doc comments.
 - <csr-id-e5a7c325b0ddd38116dbf30d5d921db42f4ac6b5/> Split PIO into multiple objects that can be moved around separately.
   One PIO block often implements multiple functions that are used in
   different parts of the codebase. Previously, that would be impossible, as
   PIO contained all StateMachine instances.
   
   Now, StateMachine instances use atomic operations whenever accessing shared
   registers, so they can be used concurrently.
 - <csr-id-49ad970d31c6d711f80dfe8cddf9688ed9b0a277/> micontroller
 - <csr-id-913c5fb0b239e7097057d28df9b892cf4aa004a9/> Fix type error
 - <csr-id-1848789ca3118279d636de10006f5cafc8338444/> Make rom_funcs functions call function instead of returning it
 - <csr-id-e44d561ef2421497fe2eeb2164a5caceea68eb94/> Add workspaces to project
 - <csr-id-a9a8df8c794c163fbb5e6d4f79f32d1196e01b28/> Add comments to rom content
 - <csr-id-6eccce595c6afb53e1708b9d68a5658d9e076619/> Change `rom_table_lookup` to use the rom's built in one
 - <csr-id-1c75ed3844f5c36cb7cb81ab0ef424a333d0fa80/> Add rom content

### Commit Statistics

<csr-read-only-do-not-edit/>

 - 1403 commits contributed to the release.
 - 70 commits were understood as [conventional](https://www.conventionalcommits.org).
 - 150 unique issues were worked on: [#104](https://github.com/winksaville/rp-hal/issues/104), [#106](https://github.com/winksaville/rp-hal/issues/106), [#107](https://github.com/winksaville/rp-hal/issues/107), [#109](https://github.com/winksaville/rp-hal/issues/109), [#110](https://github.com/winksaville/rp-hal/issues/110), [#111](https://github.com/winksaville/rp-hal/issues/111), [#112](https://github.com/winksaville/rp-hal/issues/112), [#113](https://github.com/winksaville/rp-hal/issues/113), [#116](https://github.com/winksaville/rp-hal/issues/116), [#120](https://github.com/winksaville/rp-hal/issues/120), [#121](https://github.com/winksaville/rp-hal/issues/121), [#122](https://github.com/winksaville/rp-hal/issues/122), [#123](https://github.com/winksaville/rp-hal/issues/123), [#124](https://github.com/winksaville/rp-hal/issues/124), [#131](https://github.com/winksaville/rp-hal/issues/131), [#134](https://github.com/winksaville/rp-hal/issues/134), [#135](https://github.com/winksaville/rp-hal/issues/135), [#136](https://github.com/winksaville/rp-hal/issues/136), [#146](https://github.com/winksaville/rp-hal/issues/146), [#148](https://github.com/winksaville/rp-hal/issues/148), [#151](https://github.com/winksaville/rp-hal/issues/151), [#153](https://github.com/winksaville/rp-hal/issues/153), [#162](https://github.com/winksaville/rp-hal/issues/162), [#167](https://github.com/winksaville/rp-hal/issues/167), [#170](https://github.com/winksaville/rp-hal/issues/170), [#175](https://github.com/winksaville/rp-hal/issues/175), [#177](https://github.com/winksaville/rp-hal/issues/177), [#179](https://github.com/winksaville/rp-hal/issues/179), [#180](https://github.com/winksaville/rp-hal/issues/180), [#187](https://github.com/winksaville/rp-hal/issues/187), [#189](https://github.com/winksaville/rp-hal/issues/189), [#190](https://github.com/winksaville/rp-hal/issues/190), [#192](https://github.com/winksaville/rp-hal/issues/192), [#193](https://github.com/winksaville/rp-hal/issues/193), [#195](https://github.com/winksaville/rp-hal/issues/195), [#213](https://github.com/winksaville/rp-hal/issues/213), [#217](https://github.com/winksaville/rp-hal/issues/217), [#226](https://github.com/winksaville/rp-hal/issues/226), [#233](https://github.com/winksaville/rp-hal/issues/233), [#239](https://github.com/winksaville/rp-hal/issues/239), [#258](https://github.com/winksaville/rp-hal/issues/258), [#295](https://github.com/winksaville/rp-hal/issues/295), [#298](https://github.com/winksaville/rp-hal/issues/298), [#300](https://github.com/winksaville/rp-hal/issues/300), [#301](https://github.com/winksaville/rp-hal/issues/301), [#305](https://github.com/winksaville/rp-hal/issues/305), [#312](https://github.com/winksaville/rp-hal/issues/312), [#313](https://github.com/winksaville/rp-hal/issues/313), [#314](https://github.com/winksaville/rp-hal/issues/314), [#315](https://github.com/winksaville/rp-hal/issues/315), [#318](https://github.com/winksaville/rp-hal/issues/318), [#321](https://github.com/winksaville/rp-hal/issues/321), [#328](https://github.com/winksaville/rp-hal/issues/328), [#334](https://github.com/winksaville/rp-hal/issues/334), [#336](https://github.com/winksaville/rp-hal/issues/336), [#337](https://github.com/winksaville/rp-hal/issues/337), [#338](https://github.com/winksaville/rp-hal/issues/338), [#341](https://github.com/winksaville/rp-hal/issues/341), [#344](https://github.com/winksaville/rp-hal/issues/344), [#345](https://github.com/winksaville/rp-hal/issues/345), [#346](https://github.com/winksaville/rp-hal/issues/346), [#347](https://github.com/winksaville/rp-hal/issues/347), [#350](https://github.com/winksaville/rp-hal/issues/350), [#351](https://github.com/winksaville/rp-hal/issues/351), [#352](https://github.com/winksaville/rp-hal/issues/352), [#355](https://github.com/winksaville/rp-hal/issues/355), [#357](https://github.com/winksaville/rp-hal/issues/357), [#358](https://github.com/winksaville/rp-hal/issues/358), [#359](https://github.com/winksaville/rp-hal/issues/359), [#362](https://github.com/winksaville/rp-hal/issues/362), [#363](https://github.com/winksaville/rp-hal/issues/363), [#364](https://github.com/winksaville/rp-hal/issues/364), [#365](https://github.com/winksaville/rp-hal/issues/365), [#366](https://github.com/winksaville/rp-hal/issues/366), [#367](https://github.com/winksaville/rp-hal/issues/367), [#369](https://github.com/winksaville/rp-hal/issues/369), [#371](https://github.com/winksaville/rp-hal/issues/371), [#375](https://github.com/winksaville/rp-hal/issues/375), [#378](https://github.com/winksaville/rp-hal/issues/378), [#385](https://github.com/winksaville/rp-hal/issues/385), [#386](https://github.com/winksaville/rp-hal/issues/386), [#388](https://github.com/winksaville/rp-hal/issues/388), [#396](https://github.com/winksaville/rp-hal/issues/396), [#40](https://github.com/winksaville/rp-hal/issues/40), [#401](https://github.com/winksaville/rp-hal/issues/401), [#402](https://github.com/winksaville/rp-hal/issues/402), [#422](https://github.com/winksaville/rp-hal/issues/422), [#423](https://github.com/winksaville/rp-hal/issues/423), [#429](https://github.com/winksaville/rp-hal/issues/429), [#430](https://github.com/winksaville/rp-hal/issues/430), [#431](https://github.com/winksaville/rp-hal/issues/431), [#433](https://github.com/winksaville/rp-hal/issues/433), [#434](https://github.com/winksaville/rp-hal/issues/434), [#435](https://github.com/winksaville/rp-hal/issues/435), [#436](https://github.com/winksaville/rp-hal/issues/436), [#437](https://github.com/winksaville/rp-hal/issues/437), [#438](https://github.com/winksaville/rp-hal/issues/438), [#439](https://github.com/winksaville/rp-hal/issues/439), [#44](https://github.com/winksaville/rp-hal/issues/44), [#440](https://github.com/winksaville/rp-hal/issues/440), [#441](https://github.com/winksaville/rp-hal/issues/441), [#442](https://github.com/winksaville/rp-hal/issues/442), [#443](https://github.com/winksaville/rp-hal/issues/443), [#445](https://github.com/winksaville/rp-hal/issues/445), [#447](https://github.com/winksaville/rp-hal/issues/447), [#448](https://github.com/winksaville/rp-hal/issues/448), [#450](https://github.com/winksaville/rp-hal/issues/450), [#451](https://github.com/winksaville/rp-hal/issues/451), [#457](https://github.com/winksaville/rp-hal/issues/457), [#459](https://github.com/winksaville/rp-hal/issues/459), [#463](https://github.com/winksaville/rp-hal/issues/463), [#464](https://github.com/winksaville/rp-hal/issues/464), [#487](https://github.com/winksaville/rp-hal/issues/487), [#49](https://github.com/winksaville/rp-hal/issues/49), [#491](https://github.com/winksaville/rp-hal/issues/491), [#493](https://github.com/winksaville/rp-hal/issues/493), [#50](https://github.com/winksaville/rp-hal/issues/50), [#500](https://github.com/winksaville/rp-hal/issues/500), [#504](https://github.com/winksaville/rp-hal/issues/504), [#505](https://github.com/winksaville/rp-hal/issues/505), [#510](https://github.com/winksaville/rp-hal/issues/510), [#513](https://github.com/winksaville/rp-hal/issues/513), [#52](https://github.com/winksaville/rp-hal/issues/52), [#53](https://github.com/winksaville/rp-hal/issues/53), [#534](https://github.com/winksaville/rp-hal/issues/534), [#535](https://github.com/winksaville/rp-hal/issues/535), [#54](https://github.com/winksaville/rp-hal/issues/54), [#56](https://github.com/winksaville/rp-hal/issues/56), [#585](https://github.com/winksaville/rp-hal/issues/585), [#60](https://github.com/winksaville/rp-hal/issues/60), [#61](https://github.com/winksaville/rp-hal/issues/61), [#64](https://github.com/winksaville/rp-hal/issues/64), [#68](https://github.com/winksaville/rp-hal/issues/68), [#696](https://github.com/winksaville/rp-hal/issues/696), [#71](https://github.com/winksaville/rp-hal/issues/71), [#73](https://github.com/winksaville/rp-hal/issues/73), [#74](https://github.com/winksaville/rp-hal/issues/74), [#76](https://github.com/winksaville/rp-hal/issues/76), [#78](https://github.com/winksaville/rp-hal/issues/78), [#811](https://github.com/winksaville/rp-hal/issues/811), [#817](https://github.com/winksaville/rp-hal/issues/817), [#819](https://github.com/winksaville/rp-hal/issues/819), [#822](https://github.com/winksaville/rp-hal/issues/822), [#833](https://github.com/winksaville/rp-hal/issues/833), [#86](https://github.com/winksaville/rp-hal/issues/86), [#89](https://github.com/winksaville/rp-hal/issues/89), [#91](https://github.com/winksaville/rp-hal/issues/91), [#93](https://github.com/winksaville/rp-hal/issues/93), [#94](https://github.com/winksaville/rp-hal/issues/94), [#98](https://github.com/winksaville/rp-hal/issues/98)

### Commit Details

<csr-read-only-do-not-edit/>

<details><summary>view details</summary>

 * **[#104](https://github.com/winksaville/rp-hal/issues/104)**
    - Usb fixes ([`7afa19a`](https://github.com/winksaville/rp-hal/commit/7afa19a82b9b9575cae73eedee16c4e991396784))
 * **[#106](https://github.com/winksaville/rp-hal/issues/106)**
    - Handle usb interrupt flags in driver ([`98b8e3a`](https://github.com/winksaville/rp-hal/commit/98b8e3ae9c7c299862988494f13807eb3421f949))
 * **[#107](https://github.com/winksaville/rp-hal/issues/107)**
    - Update pac so we can use rt 0.7 ([`8a42d6c`](https://github.com/winksaville/rp-hal/commit/8a42d6cf8af4849437b8cf92e412015c51d2bd85))
 * **[#109](https://github.com/winksaville/rp-hal/issues/109)**
    - Add Pico RTIC Timer Blinky Example ([`cb8dbbf`](https://github.com/winksaville/rp-hal/commit/cb8dbbf9174c8627e164315892e45ce1ccd893e8))
 * **[#110](https://github.com/winksaville/rp-hal/issues/110)**
    - Add embedded_hal::timer support ([`c509b9d`](https://github.com/winksaville/rp-hal/commit/c509b9d22f7adfe95df0d3c2537147e6c801f5fb))
 * **[#111](https://github.com/winksaville/rp-hal/issues/111)**
    - Fixed u8 overflow in spi with large postdiv ([`b399c96`](https://github.com/winksaville/rp-hal/commit/b399c96cf5ef0fcc7eb2fbe4578162c5c26f6d58))
 * **[#112](https://github.com/winksaville/rp-hal/issues/112)**
    - Add doc example for i2c ([`ac7a17f`](https://github.com/winksaville/rp-hal/commit/ac7a17f6e11acb3f16b964dcb0d0396adeac766e))
 * **[#113](https://github.com/winksaville/rp-hal/issues/113)**
    - Add basic SPI example ([`0942a17`](https://github.com/winksaville/rp-hal/commit/0942a170f149ba8adf14895bbb4d6a6d060a7728))
 * **[#116](https://github.com/winksaville/rp-hal/issues/116)**
    - Make Spi::set_baudrate public ([`be4a7e0`](https://github.com/winksaville/rp-hal/commit/be4a7e049829677d2a09551cd7ef66d454aa5ddd))
 * **[#120](https://github.com/winksaville/rp-hal/issues/120)**
    - Implements USB enumeration workaround (RP2040-E5). ([`7bfab4f`](https://github.com/winksaville/rp-hal/commit/7bfab4ffd27e93f3160bd7a449bf2a2725a9f1ee))
 * **[#121](https://github.com/winksaville/rp-hal/issues/121)**
    - Update changelog and bump verson for hal release 0.3.0 ([`b0c15cc`](https://github.com/winksaville/rp-hal/commit/b0c15ccc77395ca088917541b8e7358b5e9b62b8))
 * **[#122](https://github.com/winksaville/rp-hal/issues/122)**
    - Fix PWM set/clr_inverted ([`25e477b`](https://github.com/winksaville/rp-hal/commit/25e477b73e1399f47a7444cefc26605037804dd1))
 * **[#123](https://github.com/winksaville/rp-hal/issues/123)**
    - Implement GPIO override ([`904b6f0`](https://github.com/winksaville/rp-hal/commit/904b6f0ab9d7c5db721bfc52e596b72b2b6fc784))
 * **[#124](https://github.com/winksaville/rp-hal/issues/124)**
    - Update README with examples ([`dd3c136`](https://github.com/winksaville/rp-hal/commit/dd3c136650ef17f8b20e4b8afd15dde198cf0d3f))
 * **[#131](https://github.com/winksaville/rp-hal/issues/131)**
    - Implement embedded-hal 1.0.0-alpha.5 ([`2b6de3a`](https://github.com/winksaville/rp-hal/commit/2b6de3a3c9e5666d97a3baa7a280921a19b5b810))
 * **[#134](https://github.com/winksaville/rp-hal/issues/134)**
    - Implement bus keep inputs, as documented in C SDK ([`105dcfd`](https://github.com/winksaville/rp-hal/commit/105dcfddd70d71729cc6b809e9206243ae5cc0ab))
 * **[#135](https://github.com/winksaville/rp-hal/issues/135)**
    - Implement RngCore for RingOscillator ([`d93c4fc`](https://github.com/winksaville/rp-hal/commit/d93c4fc4c864329d936aff321ce1b419092e744b))
 * **[#136](https://github.com/winksaville/rp-hal/issues/136)**
    - Adds reset for timer, otherwise it would not run. ([`90470b6`](https://github.com/winksaville/rp-hal/commit/90470b6ff3e3aada90a0c50f221092d2d8a4c717))
 * **[#146](https://github.com/winksaville/rp-hal/issues/146)**
    - Fix i2c write read ([`ad68c9d`](https://github.com/winksaville/rp-hal/commit/ad68c9d696c2dc89d0d2a3ee07cb485e836bbee9))
 * **[#148](https://github.com/winksaville/rp-hal/issues/148)**
    - Update example feather_neopixel_rainbow.rs with new Timer syntax ([`666b22f`](https://github.com/winksaville/rp-hal/commit/666b22f56b4fde2c5b8c891fc64779c47cc2bf52))
 * **[#151](https://github.com/winksaville/rp-hal/issues/151)**
    - Add simple interrupt_disable+spinlock critical-section impl ([`d84e641`](https://github.com/winksaville/rp-hal/commit/d84e6413907a2765eb4c8dfca9aaa240d3e663b3))
 * **[#153](https://github.com/winksaville/rp-hal/issues/153)**
    - Make BSPs provide boot2 as a default feature ([`0e7abdc`](https://github.com/winksaville/rp-hal/commit/0e7abdc7050c034b9c6100336099d3cfa95b0139))
 * **[#162](https://github.com/winksaville/rp-hal/issues/162)**
    - Implement peripheral support for i2c and an advanced example ([`990d964`](https://github.com/winksaville/rp-hal/commit/990d964a93e9624cc2da8d564f8ce831ea0bfa28))
 * **[#167](https://github.com/winksaville/rp-hal/issues/167)**
    - Implements methods to allow presetting the pin state & direction ([`2eb7923`](https://github.com/winksaville/rp-hal/commit/2eb7923ebe94b8e88d0aa4a4493899f4ce563124))
 * **[#170](https://github.com/winksaville/rp-hal/issues/170)**
    - Use volatile register access for gpio interrupts ([`bac6714`](https://github.com/winksaville/rp-hal/commit/bac6714f09f887cbfc168590291c03f580bc107a))
 * **[#175](https://github.com/winksaville/rp-hal/issues/175)**
    - API to enable/disable interrupts for each PWM channel. ([`11aaf9b`](https://github.com/winksaville/rp-hal/commit/11aaf9be797511baaa7396ad146e97cf9b5d4b4e))
 * **[#177](https://github.com/winksaville/rp-hal/issues/177)**
    - Mark PIO StateMachine, Rx and Tx as Send ([`fe1e55b`](https://github.com/winksaville/rp-hal/commit/fe1e55b8c0022d3474d09ca881e9d77465698b68))
 * **[#179](https://github.com/winksaville/rp-hal/issues/179)**
    - Add PIO features required for PIO as I2C support ([`0eb65ee`](https://github.com/winksaville/rp-hal/commit/0eb65ee99bf7d074a8318dc6fb4478a8ef3f3293))
 * **[#180](https://github.com/winksaville/rp-hal/issues/180)**
    - Adds an example of using the PIO as I2C driver to control an LM75B temperature sensor ([`46e580b`](https://github.com/winksaville/rp-hal/commit/46e580b852a5d165e1211ba36e740a6e351c2066))
 * **[#187](https://github.com/winksaville/rp-hal/issues/187)**
    - Fix UART rx ([`73431a8`](https://github.com/winksaville/rp-hal/commit/73431a847b876f9604999a0e5ca9c8c6d1182e4e))
 * **[#189](https://github.com/winksaville/rp-hal/issues/189)**
    - Change UART raw read return type and fix full read ([`6d917f4`](https://github.com/winksaville/rp-hal/commit/6d917f498e7ab2f31c8047d6415cd022d09754bf))
 * **[#190](https://github.com/winksaville/rp-hal/issues/190)**
    - Document properties needed for PIO Send safety ([`f9b3d83`](https://github.com/winksaville/rp-hal/commit/f9b3d8341d9e8e83d6be89ae3692f85646bde97a))
 * **[#192](https://github.com/winksaville/rp-hal/issues/192)**
    - Adafruit ItsyBitsy RP2040 Board Support Package ([`612c44d`](https://github.com/winksaville/rp-hal/commit/612c44db46b0e8bc754b9f9191ebbce772c92efa))
 * **[#193](https://github.com/winksaville/rp-hal/issues/193)**
    - Use the PIOn peripherals in pin functions rather than creating an enum. ([`620d5f0`](https://github.com/winksaville/rp-hal/commit/620d5f0e0c3274bafafbde0cb8182ca77588ee0b))
 * **[#195](https://github.com/winksaville/rp-hal/issues/195)**
    - Pin ws2812-pio to a specific sha ([`c396423`](https://github.com/winksaville/rp-hal/commit/c396423474cb58a3141cdca1d88259590ab362c8))
 * **[#213](https://github.com/winksaville/rp-hal/issues/213)**
    - Added RtcClock DateTime and alarms ([`f68f148`](https://github.com/winksaville/rp-hal/commit/f68f148d129e0f98a975f6851def60f03b7f3d26))
 * **[#217](https://github.com/winksaville/rp-hal/issues/217)**
    - BSP for the Adafruit KB2040 ([`92f7c68`](https://github.com/winksaville/rp-hal/commit/92f7c68d5785448433a1e051443e28de24486218))
 * **[#226](https://github.com/winksaville/rp-hal/issues/226)**
    - Add basic multicore FIFO example ([`4273446`](https://github.com/winksaville/rp-hal/commit/427344667e9f24f03d132fa08e2dfaa709bc805d))
 * **[#233](https://github.com/winksaville/rp-hal/issues/233)**
    - Make fields in UartConfig public ([`24a417f`](https://github.com/winksaville/rp-hal/commit/24a417f01a9c7889099767f10ec4c8c0eeb260d2))
 * **[#239](https://github.com/winksaville/rp-hal/issues/239)**
    - Update to pio-rs v0.1.0 ([`53d9dbd`](https://github.com/winksaville/rp-hal/commit/53d9dbdf524a63ae78d06fd93e25de73aa005015))
 * **[#258](https://github.com/winksaville/rp-hal/issues/258)**
    - Add an example for accessing an SD/MMC card via SPI ([`0e3136d`](https://github.com/winksaville/rp-hal/commit/0e3136da113cd758bd95a7f66def45795cb33792))
 * **[#295](https://github.com/winksaville/rp-hal/issues/295)**
    - Add changes since 0.3.0 to changelog ([`a40bcc9`](https://github.com/winksaville/rp-hal/commit/a40bcc94ea3eb5897c7fd1b3b2c70d9563189994))
 * **[#298](https://github.com/winksaville/rp-hal/issues/298)**
    - Implement embedded-hal 1.0.0-alpha.7 traits ([`7750781`](https://github.com/winksaville/rp-hal/commit/77507816502e03f37c78ba894a364c0b454b3423))
 * **[#300](https://github.com/winksaville/rp-hal/issues/300)**
    - Add an rp2040 specific #[entry] macro. ([`f8de875`](https://github.com/winksaville/rp-hal/commit/f8de8755ccf82a782c9430c343afa8daea671b24))
 * **[#301](https://github.com/winksaville/rp-hal/issues/301)**
    - Allow to start multiple state machines in sync ([`6026ea4`](https://github.com/winksaville/rp-hal/commit/6026ea4ae37d8e1f5bad3c0361ada34beca7de58))
 * **[#305](https://github.com/winksaville/rp-hal/issues/305)**
    - Add Tiny2040 board support ([`70be6ac`](https://github.com/winksaville/rp-hal/commit/70be6ac7662a219dc1230d5c3594a33675b45aff))
 * **[#312](https://github.com/winksaville/rp-hal/issues/312)**
    - Prep for 0.4.0 release ([`b81955c`](https://github.com/winksaville/rp-hal/commit/b81955c2a828f540fd51d2273c7bd9b38c3e9584))
 * **[#313](https://github.com/winksaville/rp-hal/issues/313)**
    - Update BSPs prior to release ([`7aefb86`](https://github.com/winksaville/rp-hal/commit/7aefb8680df07f157b26bab1157e0261c70b60c3))
 * **[#314](https://github.com/winksaville/rp-hal/issues/314)**
    - Using thread send safe UART* marker, as suggested by @danielzfranklin in #Issue-284 ([`9900859`](https://github.com/winksaville/rp-hal/commit/990085948ace93cf52ff17f571dcbfc4128b880b))
 * **[#315](https://github.com/winksaville/rp-hal/issues/315)**
    - Remove some unused fields from UartPeripheral and Reader ([`f67b650`](https://github.com/winksaville/rp-hal/commit/f67b650bb38044ff009c7bbabc510de90eab4910))
 * **[#318](https://github.com/winksaville/rp-hal/issues/318)**
    - Restrict PIO FIFO writes to unsigned integers ([`e9f367f`](https://github.com/winksaville/rp-hal/commit/e9f367f26cc25b62bf228f9fb0c7eb63db2bc776))
 * **[#321](https://github.com/winksaville/rp-hal/issues/321)**
    - RAM-based interrupt vector tables ([`2bbc52f`](https://github.com/winksaville/rp-hal/commit/2bbc52ffce77d01eda8fd6c9ec348de50ad1e32e))
 * **[#328](https://github.com/winksaville/rp-hal/issues/328)**
    - Add defmt feature (as optional dep) and allow i2c::Error to be formatted ([`38692df`](https://github.com/winksaville/rp-hal/commit/38692dfcb96770a176d68cdf07ef81bcded362ab))
 * **[#334](https://github.com/winksaville/rp-hal/issues/334)**
    - Initial BSP for Pimoroni Badger2040 ([`69c2dd2`](https://github.com/winksaville/rp-hal/commit/69c2dd2c2b39a716c85b2e3c871f1614a065268d))
 * **[#336](https://github.com/winksaville/rp-hal/issues/336)**
    - Initial BSP for SparkFun Thing Plus RP2040 ([`cd69242`](https://github.com/winksaville/rp-hal/commit/cd692427f6a3dddfd180595a61625fa383587d85))
 * **[#337](https://github.com/winksaville/rp-hal/issues/337)**
    - Add the Pimoroni Plasma 2040 board ([`cf86e08`](https://github.com/winksaville/rp-hal/commit/cf86e0874984ec4105e396610de8373438a8ecb2))
 * **[#338](https://github.com/winksaville/rp-hal/issues/338)**
    - Fix typo in License section of READMEs ([`2750909`](https://github.com/winksaville/rp-hal/commit/27509090bf4f16652383996163d0829798f45d63))
 * **[#341](https://github.com/winksaville/rp-hal/issues/341)**
    - Add missing copi pin for sparkfun-pro-micro-2040 ([`a4b0486`](https://github.com/winksaville/rp-hal/commit/a4b04862ae768d326675c02c47225f8bbef04eb9))
 * **[#344](https://github.com/winksaville/rp-hal/issues/344)**
    - Add missing GPIO I2C trait implmentations ([`99b8845`](https://github.com/winksaville/rp-hal/commit/99b8845d7415875eb17e893d196db9d38bd531dc))
 * **[#345](https://github.com/winksaville/rp-hal/issues/345)**
    - Add BSP for Arduino RP2040 Nano Connect ([`882db12`](https://github.com/winksaville/rp-hal/commit/882db12855567c6b51163c5b989605d63ba5d42a))
 * **[#346](https://github.com/winksaville/rp-hal/issues/346)**
    - Add Pico PWM micro servo example ([`3842ef2`](https://github.com/winksaville/rp-hal/commit/3842ef27008d41f64005cdf4ba327f55b843bab3))
 * **[#347](https://github.com/winksaville/rp-hal/issues/347)**
    - Port HD44780 display example from rp2040-hal to rp-pico ([`f8720fc`](https://github.com/winksaville/rp-hal/commit/f8720fcbd248e69305d26b6d29e86faef6c81c3c))
 * **[#350](https://github.com/winksaville/rp-hal/issues/350)**
    - Take possible PIO program length of 32 into account ([`ed7148a`](https://github.com/winksaville/rp-hal/commit/ed7148a1e7e73cf4fb9bec97f7a331deeddf0fd1))
 * **[#351](https://github.com/winksaville/rp-hal/issues/351)**
    - Prep for HAL 0.5.0 release ([`1574a36`](https://github.com/winksaville/rp-hal/commit/1574a36f7e2971665fecf53cce98eadfa1fe9adf))
 * **[#352](https://github.com/winksaville/rp-hal/issues/352)**
    - Change pio::Tx::write to write u32 instead of <T>* ([`9641c0b`](https://github.com/winksaville/rp-hal/commit/9641c0b4a4b21ec9ffbce2a8cdbd90f629bc82ae))
 * **[#355](https://github.com/winksaville/rp-hal/issues/355)**
    - Add accessor for installed pio program offset ([`9bce594`](https://github.com/winksaville/rp-hal/commit/9bce594db2a56b12e8639dce78a5e219291939d1))
 * **[#357](https://github.com/winksaville/rp-hal/issues/357)**
    - Update dev-dependency on cortex-m-rtic to 1.1.2 ([`fa77dd5`](https://github.com/winksaville/rp-hal/commit/fa77dd54d2d933457ed79849915bf3fad7771f0b))
 * **[#358](https://github.com/winksaville/rp-hal/issues/358)**
    - Bump version of board support crates ([`6be536c`](https://github.com/winksaville/rp-hal/commit/6be536c670f43fa1db778c4f4ac4ec53b2b12846))
 * **[#359](https://github.com/winksaville/rp-hal/issues/359)**
    - Remove unused embassy/embassy-traits deps ([`1dee235`](https://github.com/winksaville/rp-hal/commit/1dee2353fa8062d52f876516287da3dfeeebef2a))
 * **[#362](https://github.com/winksaville/rp-hal/issues/362)**
    - BSP fixes ([`6ae0698`](https://github.com/winksaville/rp-hal/commit/6ae0698b7af4bbc091a03566884c47d7fc9e18d5))
 * **[#363](https://github.com/winksaville/rp-hal/issues/363)**
    - Explorer base improvements ([`0f11467`](https://github.com/winksaville/rp-hal/commit/0f114677d56c729db4a81cf420c30f54f5dc555a))
 * **[#364](https://github.com/winksaville/rp-hal/issues/364)**
    - Add bsp_pin example ([`f7cfeec`](https://github.com/winksaville/rp-hal/commit/f7cfeec0d7bddbfdb8b679641da3a155aa4ca6bf))
 * **[#365](https://github.com/winksaville/rp-hal/issues/365)**
    - Add pio pwm example ([`b12aecb`](https://github.com/winksaville/rp-hal/commit/b12aecb51c0a220f57897e8a25928de9c254027f))
 * **[#366](https://github.com/winksaville/rp-hal/issues/366)**
    - Implement embedded-hal 1.0.0-alpha.8 traits ([`99dfeaf`](https://github.com/winksaville/rp-hal/commit/99dfeaf6f28c377eab19768b03dfbbc2e4e1a654))
 * **[#367](https://github.com/winksaville/rp-hal/issues/367)**
    - Fix PIO rx fifo status ([`e5897ca`](https://github.com/winksaville/rp-hal/commit/e5897ca7a456457c63dbe9fe5ab59cb106e540c4))
 * **[#369](https://github.com/winksaville/rp-hal/issues/369)**
    - Add BSP for Seeeduino XIAO RP2040 ([`803f582`](https://github.com/winksaville/rp-hal/commit/803f582e0fd956c71459d17d42b242e95556e362))
 * **[#371](https://github.com/winksaville/rp-hal/issues/371)**
    - Add support for the Interpolator ([`31469c2`](https://github.com/winksaville/rp-hal/commit/31469c232fb054d722b4a03796e69249e87c157b))
 * **[#375](https://github.com/winksaville/rp-hal/issues/375)**
    - Wrap intrinsics docstring to avoid breakage ([`7116948`](https://github.com/winksaville/rp-hal/commit/711694881d912484b6ae947b597169c786d1511c))
 * **[#378](https://github.com/winksaville/rp-hal/issues/378)**
    - Use `ignore` instead of `text` ([`0f5bc07`](https://github.com/winksaville/rp-hal/commit/0f5bc072cdb6d51bf27d6fd236fe2faf894124f9))
 * **[#385](https://github.com/winksaville/rp-hal/issues/385)**
    - Formatting Readme ([`83b990e`](https://github.com/winksaville/rp-hal/commit/83b990ee30ec970adf0de68eff0cde4cae69db6c))
 * **[#386](https://github.com/winksaville/rp-hal/issues/386)**
    - Add docs and doc-example for Timer ([`12387bc`](https://github.com/winksaville/rp-hal/commit/12387bcf09fc0ff56f4cabaeecdb132fcbf5ba15))
 * **[#388](https://github.com/winksaville/rp-hal/issues/388)**
    - Add BSP for VCC-GND YD-RP2040 ([`b71dc36`](https://github.com/winksaville/rp-hal/commit/b71dc3678b840484f6ee71f8177efe2d8fd9c21e))
 * **[#396](https://github.com/winksaville/rp-hal/issues/396)**
    - Match Seeeduino XIAO pin name to function ([`d0eaca6`](https://github.com/winksaville/rp-hal/commit/d0eaca63ef87791caca5940726c8d2e527a1f9e6))
 * **[#40](https://github.com/winksaville/rp-hal/issues/40)**
    - Hardware divide/modulo support ([`a14cbb5`](https://github.com/winksaville/rp-hal/commit/a14cbb581907cd05208705b51b953ac773abb0d5))
 * **[#401](https://github.com/winksaville/rp-hal/issues/401)**
    - GPIO IRQ example: add check for interrupt source ([`c7acafd`](https://github.com/winksaville/rp-hal/commit/c7acafda3c6fd4d91990f76753bf211820a82038))
 * **[#402](https://github.com/winksaville/rp-hal/issues/402)**
    - Remove unnecessary cortex_m::interrupt::free in timer.rs ([`6e325ba`](https://github.com/winksaville/rp-hal/commit/6e325ba099ad472026f6abc42c3dbc637ba8e0df))
 * **[#422](https://github.com/winksaville/rp-hal/issues/422)**
    - Replace cortex_m::interrupt::Mutex with critical_section::Mutex in examples ([`51db37a`](https://github.com/winksaville/rp-hal/commit/51db37a4cb1522f28146ee1c8df82c4885ddc9bf))
 * **[#423](https://github.com/winksaville/rp-hal/issues/423)**
    - Use rp2040-hal in all example (possibly through their bsp) ([`42e929d`](https://github.com/winksaville/rp-hal/commit/42e929d7e166c04dfae41cae07ff8e215cd6e0c0))
 * **[#429](https://github.com/winksaville/rp-hal/issues/429)**
    - Remove unused dependencies & add GHA flow ([`13cad64`](https://github.com/winksaville/rp-hal/commit/13cad64c299cec7d2ea5158a254e729db12a7495))
 * **[#430](https://github.com/winksaville/rp-hal/issues/430)**
    - Prepare for HAL 0.6.0 release ([`8d52f37`](https://github.com/winksaville/rp-hal/commit/8d52f37dd1056ad3dcef78c4a74b663771a8b952))
 * **[#431](https://github.com/winksaville/rp-hal/issues/431)**
    - Add Debug and defmt::Format to the public types of rp2040_hal::gpio::dynpin ([`47d8f4f`](https://github.com/winksaville/rp-hal/commit/47d8f4fc21582ff4112dd413eacfac8da2ae4ad1))
 * **[#433](https://github.com/winksaville/rp-hal/issues/433)**
    - Temporary disable sticky-bit in set_pins too ([`dbc691f`](https://github.com/winksaville/rp-hal/commit/dbc691fb09b994ad855d4c9f0285026be846ba18))
 * **[#434](https://github.com/winksaville/rp-hal/issues/434)**
    - Fix interpolator example post migration to fugit ([`3261ecc`](https://github.com/winksaville/rp-hal/commit/3261eccd4dad0fd1e4eccf75a63574a958f5803b))
 * **[#435](https://github.com/winksaville/rp-hal/issues/435)**
    - Revert "Make Pimoroni Badger 2040's crate name consistent with it's directory" ([`4ead633`](https://github.com/winksaville/rp-hal/commit/4ead633042c1f3b9e7ba5fa1abed0758e4d28e57))
    - Make Pimoroni Badger 2040's crate name consistent with it's directory ([`1de8f90`](https://github.com/winksaville/rp-hal/commit/1de8f9016d6a94a10b8ac607f91affeaf19ddea2))
 * **[#436](https://github.com/winksaville/rp-hal/issues/436)**
    - Remove registry patches for i2c and ws2812-pio now that they are published ([`685634e`](https://github.com/winksaville/rp-hal/commit/685634e85bcd0f199fe25770f99400fa63e1aed5))
 * **[#437](https://github.com/winksaville/rp-hal/issues/437)**
    - Revert "Make Pimoroni Badger 2040's crate name consistent with it's directory" ([`4ead633`](https://github.com/winksaville/rp-hal/commit/4ead633042c1f3b9e7ba5fa1abed0758e4d28e57))
 * **[#438](https://github.com/winksaville/rp-hal/issues/438)**
    - Fix the link under the logo in rp2040-hal's readme ([`f30df4a`](https://github.com/winksaville/rp-hal/commit/f30df4a0c70d2939e7cf59cfd58882f1a4b60ee3))
 * **[#439](https://github.com/winksaville/rp-hal/issues/439)**
    - Use TimerInstant in Timer::GetCounter & add Alarm::schedule_at ([`4dbd566`](https://github.com/winksaville/rp-hal/commit/4dbd5667a635115143118825688277ff269e005d))
 * **[#44](https://github.com/winksaville/rp-hal/issues/44)**
    - PWM implementation ([`f87d7ba`](https://github.com/winksaville/rp-hal/commit/f87d7ba768af2a9324cdfa143ce1b43f1d8ae4ad))
 * **[#440](https://github.com/winksaville/rp-hal/issues/440)**
    - Add a method to allow setting the PIO's clock divisor without floats ([`0e2b4cf`](https://github.com/winksaville/rp-hal/commit/0e2b4cf7be66c7dec04ca9113f9f633c9ed3f36a))
 * **[#441](https://github.com/winksaville/rp-hal/issues/441)**
    - Use the dedicated write_bitmask_* functions ([`6d75cd8`](https://github.com/winksaville/rp-hal/commit/6d75cd82912a486151f4f1b057ee5e60e0737e98))
 * **[#442](https://github.com/winksaville/rp-hal/issues/442)**
    - Use a fixed type in Alarm::schedule ([`5ce10ff`](https://github.com/winksaville/rp-hal/commit/5ce10ff94e1f019db3a1f8beb30ba21ec0ed14a4))
 * **[#443](https://github.com/winksaville/rp-hal/issues/443)**
    - Clarify usage of boot2 section ([`9934874`](https://github.com/winksaville/rp-hal/commit/993487443a9f002094bcd10b71f2f1fb6b6478d1))
 * **[#445](https://github.com/winksaville/rp-hal/issues/445)**
    - Use rp2040_boot2::BOOT_LOADER_GENERIC_03H in the vector-table example ([`39ffe70`](https://github.com/winksaville/rp-hal/commit/39ffe70dab3cea204c930cb56043b736b438d771))
 * **[#447](https://github.com/winksaville/rp-hal/issues/447)**
    - Move interrupt related (en|dis)abling/forcing methods to the statemachine ([`322bba2`](https://github.com/winksaville/rp-hal/commit/322bba2cc0f5e1fbc1698a85c96ff2d02db03f98))
 * **[#448](https://github.com/winksaville/rp-hal/issues/448)**
    - Fix concurrent accesses to sm_execctrl and sm_instr when sideset isn't optional ([`4ddad4e`](https://github.com/winksaville/rp-hal/commit/4ddad4e74c4beed937772165c66ac0d740c5d890))
 * **[#450](https://github.com/winksaville/rp-hal/issues/450)**
    - Add the Pimoroni Servo 2040 board ([`19e2fbe`](https://github.com/winksaville/rp-hal/commit/19e2fbea1c9dd26425120939fb3d35c5614ec0fa))
 * **[#451](https://github.com/winksaville/rp-hal/issues/451)**
    - Mark Timer & Alarm* Send and Sync ([`42fc266`](https://github.com/winksaville/rp-hal/commit/42fc266e67df78286a49cf8370c1f3fc6d9d33d0))
 * **[#457](https://github.com/winksaville/rp-hal/issues/457)**
    - DMA (alternative to #209) ([`38bb05e`](https://github.com/winksaville/rp-hal/commit/38bb05e1b2b3864f267cfc426b4f5b5aaddc7cc5))
 * **[#459](https://github.com/winksaville/rp-hal/issues/459)**
    - Add rtic-monotonic support for timer & alarms (feature gated) ([`305dfc9`](https://github.com/winksaville/rp-hal/commit/305dfc9d1fbb69f4e9570b3a454cd3e3d8309498))
 * **[#463](https://github.com/winksaville/rp-hal/issues/463)**
    - Remove unused future dependency ([`eac51cd`](https://github.com/winksaville/rp-hal/commit/eac51cdd160cfd6db6937a8d22fdb76a761e823c))
 * **[#464](https://github.com/winksaville/rp-hal/issues/464)**
    - Fix watchdog counter load ([`39190c3`](https://github.com/winksaville/rp-hal/commit/39190c357f95e84947597c9f4d47193c941e965c))
 * **[#487](https://github.com/winksaville/rp-hal/issues/487)**
    - Specify required feature critical-section-impl for some examples ([`f2d9fff`](https://github.com/winksaville/rp-hal/commit/f2d9fff0e28a11bafe7862739cb05cc1ce466099))
 * **[#49](https://github.com/winksaville/rp-hal/issues/49)**
    - Clock init ([`614180e`](https://github.com/winksaville/rp-hal/commit/614180eda34d10e52d695284847ee3c96a62dd0b))
 * **[#491](https://github.com/winksaville/rp-hal/issues/491)**
    - Use i2c-pio's main branch ([`3412436`](https://github.com/winksaville/rp-hal/commit/34124363eb93a4834e12e6187f0226881d248928))
 * **[#493](https://github.com/winksaville/rp-hal/issues/493)**
    - Read ints rather than sie_status in poll ([`119534d`](https://github.com/winksaville/rp-hal/commit/119534d2dae9d286a6f3eb0f52e253777f074d89))
 * **[#50](https://github.com/winksaville/rp-hal/issues/50)**
    - Spi ([`1c6a336`](https://github.com/winksaville/rp-hal/commit/1c6a3361049777b7bf1a58767c0630dc0626e5e3))
 * **[#500](https://github.com/winksaville/rp-hal/issues/500)**
    - Add board waveshare-rp2040-zero ([`c5309f6`](https://github.com/winksaville/rp-hal/commit/c5309f6a86f4b6a49489e87fbfa6eb1dc5bcaa11))
 * **[#504](https://github.com/winksaville/rp-hal/issues/504)**
    - Update dependencies on defmt-rtt to 0.4.0 ([`d1377ac`](https://github.com/winksaville/rp-hal/commit/d1377acc19f2738c33443d313990b74ba5d8b2d8))
 * **[#505](https://github.com/winksaville/rp-hal/issues/505)**
    - Fix some clippy warnings flagged by current beta ([`0055dba`](https://github.com/winksaville/rp-hal/commit/0055dbaf875af256f8730a8130addc18df470160))
 * **[#510](https://github.com/winksaville/rp-hal/issues/510)**
    - First frame is getting lost on a USB-CDC device. ([`dfc790b`](https://github.com/winksaville/rp-hal/commit/dfc790b207eb9a10a3f75e3522d0a90b7ef50891))
 * **[#513](https://github.com/winksaville/rp-hal/issues/513)**
    - Add board waveshare-rp2040-lcd-0.96 ([`d717734`](https://github.com/winksaville/rp-hal/commit/d7177345af6b9ee01cc2d0804f6914c98463f615))
 * **[#52](https://github.com/winksaville/rp-hal/issues/52)**
    - Initial ADC impl ([`17e65c4`](https://github.com/winksaville/rp-hal/commit/17e65c4fd5101bc9cc93034aedb7b950b24751fb))
 * **[#53](https://github.com/winksaville/rp-hal/issues/53)**
    - Add 'rt' feature ([`17f8a5a`](https://github.com/winksaville/rp-hal/commit/17f8a5ab99740a071e712f342292d942ac198c86))
 * **[#534](https://github.com/winksaville/rp-hal/issues/534)**
    - Use prebuilt cargo-udeps binary in CI ([`1c6a947`](https://github.com/winksaville/rp-hal/commit/1c6a947851cd74e0d79b1267b0bf14b8a8f56b6b))
 * **[#535](https://github.com/winksaville/rp-hal/issues/535)**
    - UART DMA ([`33dd1c6`](https://github.com/winksaville/rp-hal/commit/33dd1c6f6abcdccb838a38bbf9fe409b211990d7))
 * **[#54](https://github.com/winksaville/rp-hal/issues/54)**
    - Refactor clocks ([`f310d92`](https://github.com/winksaville/rp-hal/commit/f310d92b640ffa5c92b4f05bdf121725b523762b))
 * **[#56](https://github.com/winksaville/rp-hal/issues/56)**
    - I2C ([`077cba6`](https://github.com/winksaville/rp-hal/commit/077cba68f521c5aaae099521bef58c5694b893d0))
 * **[#585](https://github.com/winksaville/rp-hal/issues/585)**
    - Rework GPIO API and fix a few inconsistencies ([`b087c0c`](https://github.com/winksaville/rp-hal/commit/b087c0c010c6c37274272bf3a0f77dc8d28a08b8))
 * **[#60](https://github.com/winksaville/rp-hal/issues/60)**
    - Add HD44780 example ([`a02c813`](https://github.com/winksaville/rp-hal/commit/a02c8131ff52da4f1f184b01056de6033facc647))
 * **[#61](https://github.com/winksaville/rp-hal/issues/61)**
    - Pwm improvements ([`ffa39f6`](https://github.com/winksaville/rp-hal/commit/ffa39f65f5005d6f44f743cded53aa679a7f5ac3))
 * **[#64](https://github.com/winksaville/rp-hal/issues/64)**
    - Improve clock frequency stuff for uninitialized clocks and add some examples ([`ffa9784`](https://github.com/winksaville/rp-hal/commit/ffa97842e295b19a01fb6438f700c683e9d90ce1))
 * **[#68](https://github.com/winksaville/rp-hal/issues/68)**
    - Add unsafe blocks around write_with_zero calls ([`5121721`](https://github.com/winksaville/rp-hal/commit/512172179a1db0810b69e927eedbae6d2ce5d677))
 * **[#696](https://github.com/winksaville/rp-hal/issues/696)**
    - Add example using GPIO DynPin ([`1c2b7a4`](https://github.com/winksaville/rp-hal/commit/1c2b7a4650c6eebe1b198d74e1cbd2bc86e0d5cc))
 * **[#71](https://github.com/winksaville/rp-hal/issues/71)**
    - Update README.md ([`553263a`](https://github.com/winksaville/rp-hal/commit/553263a5fffcf4cb410aa12bf2f066ffad852334))
 * **[#73](https://github.com/winksaville/rp-hal/issues/73)**
    - Add UART example + core::fmt support to UART ([`369ac5a`](https://github.com/winksaville/rp-hal/commit/369ac5a23ffed5395869ba430a86c40c6eba59fb))
 * **[#74](https://github.com/winksaville/rp-hal/issues/74)**
    - PIO support ([`d941f56`](https://github.com/winksaville/rp-hal/commit/d941f5637b5599b107f58215a1eb686a983e8704))
 * **[#76](https://github.com/winksaville/rp-hal/issues/76)**
    - Fix doc examples and add checking ([`d3cb29b`](https://github.com/winksaville/rp-hal/commit/d3cb29b113a90060fec9cf46d56a246c3affed42))
 * **[#78](https://github.com/winksaville/rp-hal/issues/78)**
    - Correctly configure watchdog tick generation ([`a030523`](https://github.com/winksaville/rp-hal/commit/a03052355efd58adec27240e42ce58ba3a9f5dbf))
 * **[#811](https://github.com/winksaville/rp-hal/issues/811)**
    - Add `PinGroup::set_u32` to allow setting each pin to a different state ([`549ddbf`](https://github.com/winksaville/rp-hal/commit/549ddbf190c2a8f362886409eb10784db1e1e0bc))
 * **[#817](https://github.com/winksaville/rp-hal/issues/817)**
    - Extend tests in `gpio::check_pin_groups()` ([`2e8a7d6`](https://github.com/winksaville/rp-hal/commit/2e8a7d651d5bcd6c0cf02f70f5686e4a4b65fd61))
 * **[#819](https://github.com/winksaville/rp-hal/issues/819)**
    - Install cargo-udeps and cargo-hack as binaries. ([`1d2d354`](https://github.com/winksaville/rp-hal/commit/1d2d3547f02be79553adad469953b5bae7471b78))
 * **[#822](https://github.com/winksaville/rp-hal/issues/822)**
    - Remove -Cinline-threshold=5 option from config.toml ([`956668e`](https://github.com/winksaville/rp-hal/commit/956668edc862a2b20fe97841095a2e7beac8f232))
 * **[#833](https://github.com/winksaville/rp-hal/issues/833)**
    - Re-organise Github Actions workflows. ([`32a29e0`](https://github.com/winksaville/rp-hal/commit/32a29e00dcf16b854a879334ec1681f3fb77f92f))
 * **[#86](https://github.com/winksaville/rp-hal/issues/86)**
    - Watchdog example ([`fae1caa`](https://github.com/winksaville/rp-hal/commit/fae1caaca9456320c5e329b9ae0d87001782759b))
 * **[#89](https://github.com/winksaville/rp-hal/issues/89)**
    - Multicore ([`e1f9944`](https://github.com/winksaville/rp-hal/commit/e1f99443d97a02f1f5dd5c5004bcec7b4ba97a39))
 * **[#91](https://github.com/winksaville/rp-hal/issues/91)**
    - Adafruit feather rp2040 ([`199ad89`](https://github.com/winksaville/rp-hal/commit/199ad891ed762b1b39a8cf6122998ea4d532cee5))
 * **[#93](https://github.com/winksaville/rp-hal/issues/93)**
    - Add ADC example and doc-example ([`9d2e18d`](https://github.com/winksaville/rp-hal/commit/9d2e18dc703678403abe2d33f5dd2b23532bb1e8))
 * **[#94](https://github.com/winksaville/rp-hal/issues/94)**
    - I2c lockup fix ([`301281c`](https://github.com/winksaville/rp-hal/commit/301281cba82529e9ef0017bc76842eedd8ee8262))
 * **[#98](https://github.com/winksaville/rp-hal/issues/98)**
    - Implement usb_device for rp2040 ([`db11231`](https://github.com/winksaville/rp-hal/commit/db11231f492be7eac1aa78e4644196cdc16864c8))
 * **Uncategorized**
    - Merge pull request #854 from rp-rs/fix-2350-bi ([`c8d6e7a`](https://github.com/winksaville/rp-hal/commit/c8d6e7a2d1d6a0c041cfadacc66ce812314f5108))
    - Add missing binary info to 2350 linker scripts. ([`3ef08ac`](https://github.com/winksaville/rp-hal/commit/3ef08acb18a6bd3f8e879dbdee67ee54b706620f))
    - Merge pull request #850 from jannic/embassy-executor ([`f23f877`](https://github.com/winksaville/rp-hal/commit/f23f87709dadb045a55e68937f0cda28a3bc32da))
    - Improve location of new imports ([`2289a5b`](https://github.com/winksaville/rp-hal/commit/2289a5b9da90ad28aa2a5bf75e2bb06ed66e4ac8))
    - Downgrade to embassy-executor 0.5 to avoid MSRV issues ([`1675e2c`](https://github.com/winksaville/rp-hal/commit/1675e2ca5fd7cd52a50784c34d70b1cbbc8d3b6d))
    - Use embassy-executor in rp235x examples ([`9377c4a`](https://github.com/winksaville/rp-hal/commit/9377c4a8e7df1fa520fed7b02152b54633d8cee3))
    - Use embassy-executor in rp2040 examples ([`a87830d`](https://github.com/winksaville/rp-hal/commit/a87830d0465d560ac613053c2589938ced9ad937))
    - Merge pull request #848 from jannic/replace-nostd_async ([`7816958`](https://github.com/winksaville/rp-hal/commit/78169589757e1bc5abc350909ed10c6cddfbd145))
    - Merge pull request #849 from jannic/fix-warnings ([`800dec5`](https://github.com/winksaville/rp-hal/commit/800dec590c7a2ac278553d0f1405940c0da703c6))
    - Don't allow unreachable_patterns ([`b1a5966`](https://github.com/winksaville/rp-hal/commit/b1a59660754ccecaddf10aef1f85a999b2c5227f))
    - Disable several warnings that show up with rust 1.82.0(beta) ([`fb6b977`](https://github.com/winksaville/rp-hal/commit/fb6b9773e395e4dd872f05f011ee1c6791d3ed68))
    - Tidy the code a bit ([`985274e`](https://github.com/winksaville/rp-hal/commit/985274e06bbd48d141281a065db1e89ca481a146))
    - Replace nostd_async with a simple test executor ([`0fcc24a`](https://github.com/winksaville/rp-hal/commit/0fcc24a4df5713303428b87cc7e9529a403d993b))
    - Merge pull request #835 from 9names/spibus_example ([`512b102`](https://github.com/winksaville/rp-hal/commit/512b102061e6397e46b941e2e627de313eb210b3))
    - Merge branch 'main' into spibus_example ([`ecf3fb3`](https://github.com/winksaville/rp-hal/commit/ecf3fb3fef4d0919219f4e8ab27677ab4a6046c7))
    - Merge pull request #841 from jannic/update-rp2350-uart ([`960afaf`](https://github.com/winksaville/rp-hal/commit/960afaf3cf6015f34334d03420391432dc8bc0c2))
    - Merge pull request #844 from jannic/update-pio-side-set ([`3f77ae0`](https://github.com/winksaville/rp-hal/commit/3f77ae03b02bb243c29882ab9712776a8444040f))
    - Merge pull request #845 from jannic/provide-arch-on-rp2040 ([`2c3b08c`](https://github.com/winksaville/rp-hal/commit/2c3b08cc924c11a8975cb3ba9963d9739d2a22a4))
    - Provide arch module on RP2040 ([`a8c140a`](https://github.com/winksaville/rp-hal/commit/a8c140ab57f8cf4571a032f9bae9f3417f7c21da))
    - Sync pio_side_set examples ([`f095734`](https://github.com/winksaville/rp-hal/commit/f09573492f8e96dd371df03f49c5409d3a548378))
    - Enable pull-ups in uart_loopback examples ([`0f41fd9`](https://github.com/winksaville/rp-hal/commit/0f41fd9f3fc5449d139a11d13f251dd734eeacb5))
    - Add uart_loopback example. ([`f84b764`](https://github.com/winksaville/rp-hal/commit/f84b76497648acb355ca5ca0baa1b760a3f337c0))
    - Fix typo in comment in rom_funcs ([`01b9772`](https://github.com/winksaville/rp-hal/commit/01b9772501eadc21f694349ad3c9018c0576ee38))
    - Merge pull request #842 from jannic/update-rp2350-spi ([`2d815bf`](https://github.com/winksaville/rp-hal/commit/2d815bf10790a0ddbe436a6ac9d2e6693bf742b1))
    - Port SPI changes from rp2040-hal to rp235x-hal ([`1adf2b4`](https://github.com/winksaville/rp-hal/commit/1adf2b4ae186bbff19a1c9ee1d613f6ef0d2b031))
    - Port UART updates to rp235x-hal ([`84b1753`](https://github.com/winksaville/rp-hal/commit/84b1753b4ed87ef65c5df77b2de73f8d0e6b3642))
    - Merge pull request #834 from rp-rs/add-rp235x ([`84e1bf0`](https://github.com/winksaville/rp-hal/commit/84e1bf0c82dce4b9add2a042b5a5f19f2605601d))
    - Update rp235x-hal/src/timer.rs ([`298f38b`](https://github.com/winksaville/rp-hal/commit/298f38bcee55cf0920a848356ac5e1d6c8cf92ae))
    - Update rp235x-hal/src/lposc.rs ([`8262524`](https://github.com/winksaville/rp-hal/commit/82625240aaf9d691e9c6a3ed5feb3d0ac75eb53b))
    - Merge pull request #837 from antbern/main ([`e29c2c5`](https://github.com/winksaville/rp-hal/commit/e29c2c5982bb0b6c9c1353c958dc8326529601c2))
    - Merge pull request #838 from jannic/fix_write ([`4e2f01c`](https://github.com/winksaville/rp-hal/commit/4e2f01cf3a0a13f04d2f1ae1f9a44d5d1053c62e))
    - Update rp-hal-common/src/lib.rs ([`ab006c3`](https://github.com/winksaville/rp-hal/commit/ab006c3ecd0f7626e017ad699fd15aa8ab526829))
    - Update .github/workflows/rp235x_hal_examples_riscv.yml ([`d511278`](https://github.com/winksaville/rp-hal/commit/d51127842887a8b6c19832d6ffd5651d9050ad0a))
    - Fix alloc description ([`879d831`](https://github.com/winksaville/rp-hal/commit/879d831e8800739f7bb3d1547d09bb8f28dbb2eb))
    - Fix watchdog example comments. ([`95e0529`](https://github.com/winksaville/rp-hal/commit/95e0529b624dce5ca60d71cb5d6e4020a1c48e85))
    - Fix gpio_in_out description ([`270a1db`](https://github.com/winksaville/rp-hal/commit/270a1dbb777c37d5a5ee06083b6627d14aa5990d))
    - More notes in the block-loop example. ([`6ed9f06`](https://github.com/winksaville/rp-hal/commit/6ed9f06f1cbc33f07eb16b7c79ae40225f354c42))
    - Formatting ([`aa7b66a`](https://github.com/winksaville/rp-hal/commit/aa7b66a731cb58484f75d82512f76413759ad832))
    - Mention the right board. ([`b41c5a7`](https://github.com/winksaville/rp-hal/commit/b41c5a7e56c4d31e16dc3ff43a802bb007d1e0bb))
    - Let UART write return some bytes were written ([`7a1a4fd`](https://github.com/winksaville/rp-hal/commit/7a1a4fd92bcfe6b236b98f6ff44e814ddd4ec8d8))
    - More datasheet fixes. ([`2173130`](https://github.com/winksaville/rp-hal/commit/2173130b2ca1636d75347602fc852b60a62e9e8a))
    - Switch to using picotool ([`17296c7`](https://github.com/winksaville/rp-hal/commit/17296c75df1a9d245c0d82ac2d97a2215ce27234))
    - Datasheet link clean-ups ([`86b4e69`](https://github.com/winksaville/rp-hal/commit/86b4e69306a26630483e455e50f5c97bcffa88e6))
    - Implement `embedded_io` `ReadReady` and `WriteReady` traits for uart ([`07166ed`](https://github.com/winksaville/rp-hal/commit/07166ed3ba055820fbcfce463415f4816a34eda8))
    - Use hal::Timer to be consistent ([`466be69`](https://github.com/winksaville/rp-hal/commit/466be690bb8155bf6759983dad46fd414d7d2ccc))
    - Rename binding pac->p ([`5124f5d`](https://github.com/winksaville/rp-hal/commit/5124f5d8d32b54e63a607e9a576f2b04a46ecd3a))
    - Added even more comments to spi_eh_bus. ([`7ae4610`](https://github.com/winksaville/rp-hal/commit/7ae4610bbdc119d71b76bc0000e64feea0ade77e))
    - Impl some review fixes ([`3d89e33`](https://github.com/winksaville/rp-hal/commit/3d89e339da8d3a3717a7367272d3ef59dc88d07d))
    - Fix up the SPI example pins comment too ([`bb8c6a0`](https://github.com/winksaville/rp-hal/commit/bb8c6a096733bc6bf890dc81a49021a3d990358b))
    - Add SPI example using embedded_hal_bus ([`2b63ab2`](https://github.com/winksaville/rp-hal/commit/2b63ab2a107e13be09ee79f08df91b4cc9918529))
    - Use published 2350 PAC. ([`4d2d08f`](https://github.com/winksaville/rp-hal/commit/4d2d08fa5e9df43f0332d3d2fe5ad7e436ee5c8d))
    - Format rp235x-hal/Cargo.toml ([`2589e20`](https://github.com/winksaville/rp-hal/commit/2589e201af21f1478b293a318083d3e8567930df))
    - Don't check udeps for RISC-V examples ([`94b2317`](https://github.com/winksaville/rp-hal/commit/94b231765fbcddc15915b673a1f739c1d19e6fb6))
    - Set the rp235x-hal-examples to build in ARM mode by default ([`650a608`](https://github.com/winksaville/rp-hal/commit/650a60840235aef5f3e1dfd88b8e61b9c53aa2cf))
    - Moved some UART stuff into rp-hal-common. ([`4f07e93`](https://github.com/winksaville/rp-hal/commit/4f07e9366c3b0433d774b244f9c88aa366476d79))
    - Add an RP2350 HAL. ([`5cb6f9e`](https://github.com/winksaville/rp-hal/commit/5cb6f9eba15ecfcdcb46e5dd480d0708c9e74a87))
    - Merge pull request #828 from rp-rs/move-examples-delete-workspace ([`679ed27`](https://github.com/winksaville/rp-hal/commit/679ed272b03a5a6baf574ff9cfe49f1845a911fd))
    - Reformat all Cargo.toml files ([`fae6b25`](https://github.com/winksaville/rp-hal/commit/fae6b2507abfe65f21a53ec320b3728f65341f01))
    - Bump to GHA checkout@v4 ([`e5fcde3`](https://github.com/winksaville/rp-hal/commit/e5fcde3140ac59d8cd00d02d13de683c8e6e0ac9))
    - Deletes the top-level workspace and moves the examples. ([`b31683c`](https://github.com/winksaville/rp-hal/commit/b31683c62907a20763f7314c67f19b1c1d470eae))
    - Merge pull request #830 from Dirbaio/rp-binary-info ([`103e4fa`](https://github.com/winksaville/rp-hal/commit/103e4fa40ce409defdafd91e19e2ee77edca71f3))
    - Always export binary-info crate as a module. ([`8a7b4ec`](https://github.com/winksaville/rp-hal/commit/8a7b4ece9d5424d714143d45dec5509e76b53482))
    - Extract picotool binary info to a separate `rp-binary-info` crate. ([`5380a65`](https://github.com/winksaville/rp-hal/commit/5380a6517279b6364c55625d1dacf5ab08a967a6))
    - Merge pull request #831 from ithinuel/move-spi-set-format-to-any-state ([`903376a`](https://github.com/winksaville/rp-hal/commit/903376aa26788e6cfbff663214424b59bd21435a))
    - Fix comment typo in rp2040-hal/src/spi.rs ([`1e06c4f`](https://github.com/winksaville/rp-hal/commit/1e06c4f81752ceec2b15e3130343606028d41d60))
    - Move set_format to all states ([`f801611`](https://github.com/winksaville/rp-hal/commit/f8016112933d1d746baa539f27e8f4363ed5804d))
    - Merge pull request #829 from rp-rs/fix-apache-text ([`5eeaca4`](https://github.com/winksaville/rp-hal/commit/5eeaca4a120da8b5427e2667ffebd00c5dd1b852))
    - Switch to the longer contribution text. ([`cb94933`](https://github.com/winksaville/rp-hal/commit/cb9493324cf43608903a0ecefaa2ffd7fcfe7100))
    - Rationalise all the license files and copyright notices. ([`41b5c8c`](https://github.com/winksaville/rp-hal/commit/41b5c8c01872874dd07e04849495ed39dc75f55f))
    - Merge pull request #824 from rp-rs/add-picotool-metadata-again ([`23a68bc`](https://github.com/winksaville/rp-hal/commit/23a68bce0b914eff13a0e750ba22b0d3f616e06a))
    - Adds binary info block support. ([`e878daf`](https://github.com/winksaville/rp-hal/commit/e878daf624dd4413512b162cd53116c9392ceca7))
    - Merge pull request #798 from jannic/issue-782 ([`885de2e`](https://github.com/winksaville/rp-hal/commit/885de2ea0730d02d03a12765d3ac3ef212aceb68))
    - Merge pull request #800 from jannic/test-for-pr799 ([`186cce2`](https://github.com/winksaville/rp-hal/commit/186cce2c4e9021eb81ca7a39ced526e702dd5bc3))
    - This adds a test-case covering the fix from PR #799 ([`b142a7b`](https://github.com/winksaville/rp-hal/commit/b142a7bb807e7dbc1b9a0d786d990eb269a59e23))
    - Merge pull request #818 from hfly0/feat/rtc_error_defmt_impl ([`fc72c25`](https://github.com/winksaville/rp-hal/commit/fc72c252b866bd7921d3d1cfe27fa983c3120f36))
    - Merge pull request #815 from jannic/issue-216 ([`5da290a`](https://github.com/winksaville/rp-hal/commit/5da290a9e375ef86dda57d5639f0cf75f425f74e))
    - Derive `defmt::Format` for `RtcError`, fix doc typo ([`fa584e6`](https://github.com/winksaville/rp-hal/commit/fa584e6010d5b6315bbda72892fe0507fd005323))
    - Merge pull request #814 from jannic/uart_example_comments ([`a09724f`](https://github.com/winksaville/rp-hal/commit/a09724f8987530c650c70dec24d6b2d51ec4d5ca))
    - Base CountDown on Timer instead of &Timer ([`e4a722d`](https://github.com/winksaville/rp-hal/commit/e4a722dd629985f14efc5609b4579ef2cc0bae80))
    - Add some comments to the UART DMA example ([`df4d971`](https://github.com/winksaville/rp-hal/commit/df4d971869fd6538cef449875de8ae9440e5b023))
    - Merge pull request #813 from jannic/fix-beta-clippy-warnings ([`2d593e4`](https://github.com/winksaville/rp-hal/commit/2d593e414cc90a18a035c857d94d4b54f71f03c9))
    - Fix some indentations in doc comments flagged by clippy in beta ([`5c636d4`](https://github.com/winksaville/rp-hal/commit/5c636d4d33e56cc84ce151b274d5fd38f949665e))
    - Merge pull request #812 from jannic/fix-pin-group-write ([`1da07a0`](https://github.com/winksaville/rp-hal/commit/1da07a03665c5cf4d730fe9a80d73cee72bfea97))
    - Fix writing to pin groups ([`74b64b3`](https://github.com/winksaville/rp-hal/commit/74b64b341c6f30a8a66439762757ced7370e8eda))
    - Merge pull request #802 from jannic/fix-lints ([`6263d70`](https://github.com/winksaville/rp-hal/commit/6263d70ff4d9207ab9224cf8c72eb25bbf4ce51f))
    - Merge pull request #809 from jannic/issue-806 ([`d84ed8b`](https://github.com/winksaville/rp-hal/commit/d84ed8baf243841355c5e602fe45af8a7d7982d9))
    - Enable common features in example build command. ([`16a8aa6`](https://github.com/winksaville/rp-hal/commit/16a8aa6b5a57df11b5a501bbee738e720fe4d788))
    - Merge pull request #803 from EliseZeroTwo/elisezerotwo/dma_abort ([`e4e909e`](https://github.com/winksaville/rp-hal/commit/e4e909e3abb609fa9413cdbd8b68d60e0f98528d))
    - Add support for aborting DMA transfers ([`b830913`](https://github.com/winksaville/rp-hal/commit/b83091377ffc7b671c19dcefc1d9257e4c52910e))
    - Merge pull request #807 from martinsp/fix-output-pin-eh1 ([`a1150d5`](https://github.com/winksaville/rp-hal/commit/a1150d5366f0cc9b8fede2f2e10a993ef46f5f74))
    - Fix set_low() and set_high() implementation for OutputPin ([`8164340`](https://github.com/winksaville/rp-hal/commit/8164340e066463ba2914387ad7743d1f1ec037a7))
    - Avoid discarding already read bytes on error ([`4c50e94`](https://github.com/winksaville/rp-hal/commit/4c50e944bb018881e68c0f3a39462f7cd443277b))
    - Merge pull request #805 from jannic/fix-transmutes ([`d152844`](https://github.com/winksaville/rp-hal/commit/d15284402c80d9cc564e5bf1a7e2db2c43be02b1))
    - Fix formatting in pin_sealed.rs ([`6ec57de`](https://github.com/winksaville/rp-hal/commit/6ec57de812eb8df72e304d083f0ce762101bcec5))
    - Fix some clippy lints triggered by rust beta ([`7aae5e3`](https://github.com/winksaville/rp-hal/commit/7aae5e3dc8b913e7369453abe8ec2416e25203f5))
    - Fix transmutes ([`b02c28f`](https://github.com/winksaville/rp-hal/commit/b02c28f6f034b411c2e6ca38d2d6fcc10b1ce5ca))
    - Merge pull request #804 from jannic/probe-rs-install ([`a1b20f3`](https://github.com/winksaville/rp-hal/commit/a1b20f3a2cc0702986c478b0e1ee666f44d66853))
    - Update install instructions for probe-rs ([`02c816d`](https://github.com/winksaville/rp-hal/commit/02c816db74b8183039a07c5ddc30fe47e7e2de4d))
    - Merge pull request #799 from mjptree/fix-oneshot-adc ([`dfbdb9a`](https://github.com/winksaville/rp-hal/commit/dfbdb9ae667b09fc72290377e19189daac9ad0f6))
    - Fix oneshot adc read waiting indefinitely ([`a6f43a4`](https://github.com/winksaville/rp-hal/commit/a6f43a49928f6a0a5f7d94f3ac881a671a68f85d))
    - Merge pull request #700 from ithinuel/add-send-break ([`840e90b`](https://github.com/winksaville/rp-hal/commit/840e90b973669e08f509b32bfd92ede5a8ff5d8f))
    - Merge pull request #781 from jannic/embedded_io_reader_weiter ([`9306210`](https://github.com/winksaville/rp-hal/commit/9306210eaf6f06b66f0bc8937ff842d752ebe1d8))
    - Merge pull request #785 from jannic/fix_halt ([`cdc542f`](https://github.com/winksaville/rp-hal/commit/cdc542f922e8ff44ae5bc2d03ae4fd578480f961))
    - Merge pull request #792 from jannic/improve-deprecation-note ([`548f82a`](https://github.com/winksaville/rp-hal/commit/548f82a8c9ce6b8a6a125c227b2ee0ff4e9a223c))
    - Slightly improve deprecation note on from_program ([`48dbfcc`](https://github.com/winksaville/rp-hal/commit/48dbfcc3de2c5e80c84a8726d6dd98818b1635c8))
    - Implement `send_break` support ([`8e15127`](https://github.com/winksaville/rp-hal/commit/8e151273b597f4e2cada17b5bcfc73a687af8d7a))
    - Merge pull request #790 from jsgf/move-dma-transfersize ([`8adec5a`](https://github.com/winksaville/rp-hal/commit/8adec5ae6731def490d8702eef4b7b09e8cfc271))
    - Move TransferSize to `dma` module ([`efe574a`](https://github.com/winksaville/rp-hal/commit/efe574af0aefa84585ed2ea4a5e0c60916b118c5))
    - Merge pull request #788 from jsgf/pio-dma-size ([`616f6bc`](https://github.com/winksaville/rp-hal/commit/616f6bc853e04f83f2f73fbcac66f7de782a813b))
    - Fix Tx::transfer_size ([`36a05f2`](https://github.com/winksaville/rp-hal/commit/36a05f24618ded177bf3b51a082e37ca4669243d))
    - Remove type params on `build` to avoid inference failures ([`caaef72`](https://github.com/winksaville/rp-hal/commit/caaef7224a84465e0e7f4d42f9d228bb78d9318c))
    - Add some more type params ([`6ce5672`](https://github.com/winksaville/rp-hal/commit/6ce5672f62bc0ba8a64c67c6e8d40375d1fa2309))
    - Enable transfer size of PIO DMA to be specified ([`9947302`](https://github.com/winksaville/rp-hal/commit/9947302a62b1a9c3d70f598199751c38f4c55a52))
    - Merge pull request #787 from Text-Input/fix_rom_float ([`7f13938`](https://github.com/winksaville/rp-hal/commit/7f13938c8d4d8199cf31cff836ff48fd870bd8d3))
    - Fix float_to_fix64 return value & docs for f32 trig functions ([`caa0ea0`](https://github.com/winksaville/rp-hal/commit/caa0ea028fbe72035c6c8fea99d00a791140065c))
    - Fix debugging after halt() ([`effcc46`](https://github.com/winksaville/rp-hal/commit/effcc46b1d2e4e6e490a5384e6e5c9ed51c7267f))
    - Merge pull request #783 from jannic/div_ceil ([`50865b7`](https://github.com/winksaville/rp-hal/commit/50865b705d9a315813fac86a4bee060d3f4282aa))
    - Simplify ceiling division in delay calculation ([`4a677a6`](https://github.com/winksaville/rp-hal/commit/4a677a69ae07cbb52881bbda86e4947afc5fa14d))
    - Implement embedded_io traits for Reader/Writer ([`0d819d3`](https://github.com/winksaville/rp-hal/commit/0d819d3d55195ada874ece21e23250bd793763bf))
    - Merge pull request #775 from jannic/prepare-0.10.0 ([`413420a`](https://github.com/winksaville/rp-hal/commit/413420acdb24760f8c3bb9cdb99a408ffa73bfcb))
    - Add some missing changelog entries ([`492b8f5`](https://github.com/winksaville/rp-hal/commit/492b8f55e69df4a5715e10c26dc4d6de3e3f92be))
    - Optimistically set release date to today in CHANGELOG.md ([`b37424d`](https://github.com/winksaville/rp-hal/commit/b37424da1238293436efa18002e8bf760f978fca))
    - Update version numbers to 0.10.0 ([`a036d98`](https://github.com/winksaville/rp-hal/commit/a036d987a629fd67a5d20c37ec19fb501b95413a))
    - Update CHANGELOG.md ([`a6c53ce`](https://github.com/winksaville/rp-hal/commit/a6c53ce78337e21359b318b8a082289a8d7ded42))
    - Merge pull request #779 from jannic/clippy ([`f1a98fd`](https://github.com/winksaville/rp-hal/commit/f1a98fd7a9d61ffd50666808fc7565edf6f6d3e2))
    - Remove redundant imports ([`745c9dc`](https://github.com/winksaville/rp-hal/commit/745c9dcef3f97e66f9eb99d497c1594a24fff342))
    - Implement Default for structs which have a no-argument new() constructor ([`b46447b`](https://github.com/winksaville/rp-hal/commit/b46447bb2fdde3e4e621be0476e6cbcbac1e2fdc))
    - Merge pull request #778 from jannic/clippy ([`c859b7f`](https://github.com/winksaville/rp-hal/commit/c859b7f2cdca399aecd5f61d82e877131a4a866f))
    - Resolve warnings shown by cargo doc ([`a94ff26`](https://github.com/winksaville/rp-hal/commit/a94ff268d7c8192e116e65f80a53fa3e4002d5c4))
    - Resolve warnings detected by cargo +nightly clippy ([`2a65b6d`](https://github.com/winksaville/rp-hal/commit/2a65b6d176cb08b03ff2dc2d38301318cf033cc4))
    - Merge pull request #701 from andrewh42/wake-from-dormant ([`1000a10`](https://github.com/winksaville/rp-hal/commit/1000a10dcdb3d61e067941ee578211feef60e2c9))
    - Merge pull request #755 from jannic/issue-754 ([`556dddd`](https://github.com/winksaville/rp-hal/commit/556dddd7327724638a44b7d0b40847df29bb0414))
    - Update for recent HAL API changes ([`0b274b6`](https://github.com/winksaville/rp-hal/commit/0b274b65ffdf68f6f22b2b5e525d527356ded988))
    - Merge branch 'main' into wake-from-dormant ([`9e1e9d5`](https://github.com/winksaville/rp-hal/commit/9e1e9d5a77a086dc9e57782a8c948d43ea64881d))
    - Add documentation ([`6279f2b`](https://github.com/winksaville/rp-hal/commit/6279f2b31d7ce77da31b25ae0a31938e18d1c39a))
    - Add on-target test ([`ffaa072`](https://github.com/winksaville/rp-hal/commit/ffaa0724ddae406f5f3e43bd33f18be868c54071))
    - Disable input enable for all gpio pins after bringing pads out of reset ([`b922aae`](https://github.com/winksaville/rp-hal/commit/b922aae99c37e66ccfc81604a02fac3cc1b3b943))
    - Disable input enable for ADC pins after bringing pads out of reset ([`6d8d3aa`](https://github.com/winksaville/rp-hal/commit/6d8d3aace96b1f67801593b9017ae0de66e12ffd))
    - Set input_enable when selecting GPIO function ([`545fbbd`](https://github.com/winksaville/rp-hal/commit/545fbbd9b5de032e4201d7700c18e800e708a46a))
    - Merge pull request #777 from AkiyukiOkayasu/fix-typo ([`a9af216`](https://github.com/winksaville/rp-hal/commit/a9af2163d03de147277e44b3d28c566868292ecc))
    - Fix typo ([`93663a1`](https://github.com/winksaville/rp-hal/commit/93663a18d5687b6f730f9adbefeacae013b8b0ea))
    - Merge pull request #757 from AkiyukiOkayasu/vreg ([`deca3a5`](https://github.com/winksaville/rp-hal/commit/deca3a590cc0a5e0dc2b10202b200fcb0d779cc4))
    - Remove on-target-test for vreg voltage ([`6c5db05`](https://github.com/winksaville/rp-hal/commit/6c5db059bbe6ce8afdc9650f155953abdc9ef512))
    - Add on-target-test for vreg voltage ([`2912d43`](https://github.com/winksaville/rp-hal/commit/2912d43128cb887293a19e0a48eb1903b98ad9c9))
    - Refactor set_voltage() and get_voltage() ([`4adab0d`](https://github.com/winksaville/rp-hal/commit/4adab0d40697cf4341dd0553f5e48342b2f1ed3d))
    - Merge remote-tracking branch 'origin' into vreg ([`4255aa1`](https://github.com/winksaville/rp-hal/commit/4255aa14dd85ec4d8ae83543bbfc44912806fdd5))
    - Merge pull request #776 from jannic/as_ptr ([`a9b91ea`](https://github.com/winksaville/rp-hal/commit/a9b91ea50655ace5067da8dec488681c9d53ebae))
    - Merge pull request #739 from jannic/adc-fifo ([`2987210`](https://github.com/winksaville/rp-hal/commit/29872106d82b0457dffaf688c89c78d8bc3a904d))
    - Revert unrelated changes to example to ease review ([`f7e521d`](https://github.com/winksaville/rp-hal/commit/f7e521dbe0d29ded3fa6e2287c677ed3e419d107))
    - Fix examples ([`48a870f`](https://github.com/winksaville/rp-hal/commit/48a870f8d0c0d4140c01673b4a8773e831cbbf51))
    - Free_running() should take an AdcChannel ([`202c1d3`](https://github.com/winksaville/rp-hal/commit/202c1d341f55691920b7fa71d53737ef4fc6755b))
    - Fix code example in docs ([`0667ce8`](https://github.com/winksaville/rp-hal/commit/0667ce85786c5ce9958b5cdda7dffd192e7e7839))
    - Update changelog ([`9c6c45b`](https://github.com/winksaville/rp-hal/commit/9c6c45b1a5d759612cb7e1570a66f0ae16125774))
    - Improve docs ([`7f5c710`](https://github.com/winksaville/rp-hal/commit/7f5c7102ab7c30842bd6e25864beff3d6c29f9d5))
    - Use AdcChannel to implement RoundRobin ([`4ca2503`](https://github.com/winksaville/rp-hal/commit/4ca2503a272dec6cfb334d72facdd365f38ef126))
    - New trait AdcChannel to represent AdcPin and TempSense ([`63db28f`](https://github.com/winksaville/rp-hal/commit/63db28f400e75751f505adfe0d79a367474c635c))
    - Allow free-running ADC mode without FIFO ([`1f341fd`](https://github.com/winksaville/rp-hal/commit/1f341fd4936c4b41933ec669d97fe0a084fb1bc6))
    - Use as_ptr() to retrieve pointer to register ([`c0679ca`](https://github.com/winksaville/rp-hal/commit/c0679ca582ea355181db5daf5145d1dd1de5ac2b))
    - Merge pull request #770 from AkiyukiOkayasu/update-pac-v06 ([`c11fed9`](https://github.com/winksaville/rp-hal/commit/c11fed9b0dc11f19dc19f89e0c0b79e09c2f65e3))
    - Update to rp2040-pac 0.6.0 ([`55fa8dd`](https://github.com/winksaville/rp-hal/commit/55fa8ddeac603d400d4883f0b77e983e316da101))
    - Merge pull request #773 from rp-rs/update-vco-min-frequency ([`6a90750`](https://github.com/winksaville/rp-hal/commit/6a90750a5f06aa89f051360c28e08ed188ea6aa3))
    - Update VCO minimum frequency ([`4ef7689`](https://github.com/winksaville/rp-hal/commit/4ef768968a120cbaae3a9e6e0d77b69c1da627ea))
    - Merge pull request #765 from ithinuel/i2c-impl-i2c-write-iter ([`54e6cfa`](https://github.com/winksaville/rp-hal/commit/54e6cfabdf804c9dfdeea9fea9692c0df7e05110))
    - Fix a bug in retrieving register addresses ([`3685733`](https://github.com/winksaville/rp-hal/commit/368573354fdbb7f3c433e48c7985a05232155fd2))
    - Update rp2040-pac dependency to latest version of rp-rs ([`e0ddd91`](https://github.com/winksaville/rp-hal/commit/e0ddd9157c38fa43c2c17a4823c05fa9e1f17825))
    - Merge pull request #1 from jannic/pr-770-fix-spi-dma ([`c6d24bc`](https://github.com/winksaville/rp-hal/commit/c6d24bce0afbd3dae938ac9af297353d145159f8))
    - Fix SPI DMA ([`ad1d491`](https://github.com/winksaville/rp-hal/commit/ad1d491a3d2e869bb0eb19deaddef0416111e36b))
    - Necessary changes to example with pac updates ([`bd428da`](https://github.com/winksaville/rp-hal/commit/bd428da43df775eba855fcb9c52af119359d532d))
    - Undo changes made by mistake ([`552ddc0`](https://github.com/winksaville/rp-hal/commit/552ddc08da5d0b817bce8c2cc780f50678c6ffc7))
    - Use regenerated pac by adding --reexport-interrupt to svd2rust ([`aae472d`](https://github.com/winksaville/rp-hal/commit/aae472d1c70b93ca7c016d433fae4ab730d2811b))
    - Clippy ([`1f41683`](https://github.com/winksaville/rp-hal/commit/1f41683ee369a5b90814768dc7050e6c276c430a))
    - Minor modifications due to pac updates ([`2c46a9f`](https://github.com/winksaville/rp-hal/commit/2c46a9fd069ab7db09ad50cd8d7ecc15fd0f32f5))
    - Use a fixed pac that CorePeripherals re-exports ([`6154529`](https://github.com/winksaville/rp-hal/commit/61545294be12f4871d0afdf3a0ac6e74facd93a5))
    - Updates necessary because of rp2040-pac update ([`366d149`](https://github.com/winksaville/rp-hal/commit/366d1496c771f1fc395be07572ab77607a00c955))
    - Update ([`e917138`](https://github.com/winksaville/rp-hal/commit/e9171381b67795ea559d451b61eaf3bc61c911c8))
    - Update ([`8603abd`](https://github.com/winksaville/rp-hal/commit/8603abd0f4578eef2579654949e076bf49e6fe5d))
    - Updates ([`88aedf5`](https://github.com/winksaville/rp-hal/commit/88aedf53a45d4b432c8318e26aba73a28c6c20fa))
    - Updates necessary because of rp2040-pac update ([`684a312`](https://github.com/winksaville/rp-hal/commit/684a31206fa7f41bb3b6329414bf6f9bc4aa70ff))
    - Add patch section to use updated rp2040-pac ([`65309ff`](https://github.com/winksaville/rp-hal/commit/65309ff742e03ae84a1ae31ecb9b135d06cbe7b1))
    - Merge pull request #769 from rursprung/add-cargo-categories-and-keywords ([`e175d2a`](https://github.com/winksaville/rp-hal/commit/e175d2a4865a42f75f84fde4682eae7cc41d8daf))
    - Add `categories` & `keywords` ([`bb7a98e`](https://github.com/winksaville/rp-hal/commit/bb7a98e3af8d9ca661b3f9be0375355a55f91cee))
    - Merge pull request #768 from ithinuel/add-getters-to-gpio-pads ([`9296ebc`](https://github.com/winksaville/rp-hal/commit/9296ebc7669611724ef725dc55ed9cba18548edc))
    - I2c async: simplify transaction_iter ([`edc3443`](https://github.com/winksaville/rp-hal/commit/edc34435ebd816742e9d268961de87fba8277c4c))
    - Missed documentation update in copy/pase ([`c99bf2a`](https://github.com/winksaville/rp-hal/commit/c99bf2abd5799bb7fd54af5e6a2d8a1a17864781))
    - Add getters to the various pad overrides (not type tracked) ([`821909a`](https://github.com/winksaville/rp-hal/commit/821909ae812ece13c2f7c0deafdc0a4a5923b4e3))
    - Merge pull request #306 from umgefahren/feature/AllocExampleRpPico ([`099e34f`](https://github.com/winksaville/rp-hal/commit/099e34fb1f8a7c5f00cc3b3259e1c4570c67bfb4))
    - Switch from alloc-cortex-m to embedded-alloc ([`c161847`](https://github.com/winksaville/rp-hal/commit/c161847c1b4c6092990ccffc5e0b08cf0a6f3c3e))
    - Reduce the number of spurious irq ([`4c72824`](https://github.com/winksaville/rp-hal/commit/4c72824859b6b2b229a1a3409132b26887619c0d))
    - Add an i2c-write-iter test for async ([`ed7bfd9`](https://github.com/winksaville/rp-hal/commit/ed7bfd9623f9105d6f1b78aa26eb2bd985e69b0c))
    - Update alloc example for embedded-hal 1.0 ([`fccfdbe`](https://github.com/winksaville/rp-hal/commit/fccfdbebd214e97e67043ac39258f777b3b0b97e))
    - Merge pull request #767 from jannic/rename-config ([`a650b00`](https://github.com/winksaville/rp-hal/commit/a650b002130702c8e140e6f95ec878ed2a4826d0))
    - Added an example for using alloc-cortex-m ([`89cabdf`](https://github.com/winksaville/rp-hal/commit/89cabdf0cfbd06a99e5d782ac0dd572e1dfacf9a))
    - Rename .cargo/config to .cargo/config.toml ([`909af88`](https://github.com/winksaville/rp-hal/commit/909af88e9fce1e254993fc1da7dd3269098931e9))
    - Implement i2c-write-iter traits ([`6ad3d1e`](https://github.com/winksaville/rp-hal/commit/6ad3d1e71ad1eba163cdb62fd3f08d26495b72f9))
    - Merge pull request #747 from ithinuel/introduce-async-i2c ([`07ba575`](https://github.com/winksaville/rp-hal/commit/07ba575466bd68b4364e10fd277e6f931d3480c1))
    - Merge pull request #763 from ithinuel/bump-rustc-nightly-for-cargo-udeps ([`d3a2f68`](https://github.com/winksaville/rp-hal/commit/d3a2f68770781ed9fe8054c8e9c34b36fa679cf9))
    - Implement embedded-hal-async with tests ([`7a47574`](https://github.com/winksaville/rp-hal/commit/7a47574795504a42ba2892ffa883338337ccaae5))
    - Add on-target-tests & fix discovered issues ([`7d1bd63`](https://github.com/winksaville/rp-hal/commit/7d1bd63e57dc8f1e1a78797c0a5875b19391f75f))
    - Merge pull request #762 from ithinuel/move-on-target-tests ([`31ccfa3`](https://github.com/winksaville/rp-hal/commit/31ccfa3a5dddfd903b4b2b0725faa620e69441ac))
    - Merge pull request #761 from ithinuel/bump_msrv ([`6715d71`](https://github.com/winksaville/rp-hal/commit/6715d71728937681e1c8d3e0ea9724c271a808e5))
    - Bump cargo-hack & cargo-udeps versions & nightly for cargo-udeps ([`2c451ac`](https://github.com/winksaville/rp-hal/commit/2c451ac0a5f3296df8a14e2103d02bee20ab3c0a))
    - Move on-target-tests back to the workspace ([`b53f51d`](https://github.com/winksaville/rp-hal/commit/b53f51db60f7411ccd243f315982dd49f5d1b5dc))
    - Bump msrv from 1.65 to 1.75 ([`2838f1d`](https://github.com/winksaville/rp-hal/commit/2838f1d999443a18e77daef61c715018c45e86c5))
    - Add on-chip voltage regulator (VREG) voltage setting function ([`77d13b8`](https://github.com/winksaville/rp-hal/commit/77d13b8dc9835d40eec9b980e4a7cb8cc48257ef))
    - Merge pull request #753 from jannic/eh10 ([`1481429`](https://github.com/winksaville/rp-hal/commit/1481429255f518f4a481395bd4a157c9d482fec1))
    - Implement inherent functions for the watchdog ([`da0dfe5`](https://github.com/winksaville/rp-hal/commit/da0dfe5d83355e87532c62b874b50097271da667))
    - :spi::MODE_0 -> embedded_hal::spi::MODE_0 ([`4480c1d`](https://github.com/winksaville/rp-hal/commit/4480c1d6f8fb13c1bf1aff69be28012c11e6ec1c))
    - Work on timer docs ([`4f8e6cd`](https://github.com/winksaville/rp-hal/commit/4f8e6cd069a5fb594fa559437fe3872f3db5345b))
    - Change the examples to use EH 1.0 traits where possible. ([`2e5237a`](https://github.com/winksaville/rp-hal/commit/2e5237a057d67ce3cceb35a5082955577b8ac749))
    - Add 1.0 impls for InOutPin. ([`d1c49ae`](https://github.com/winksaville/rp-hal/commit/d1c49ae0c9a06cbf27ec2b75c529fef7d73a78ed))
    - Update embedded-hal naming in peripheral.rs ([`e8bff0c`](https://github.com/winksaville/rp-hal/commit/e8bff0c627464ce1730f22274dc702907054fbed))
    - Update embedded-hal naming in writer.rs ([`64762e3`](https://github.com/winksaville/rp-hal/commit/64762e39c1bd50ebe3e21dd3870c76ad01cfeb92))
    - Update embedded-hal naming in reader.rs ([`00e27a8`](https://github.com/winksaville/rp-hal/commit/00e27a899144af1dbd534d8164a99a18e694d41b))
    - Another tiny improvement in spi.rs ([`d533dab`](https://github.com/winksaville/rp-hal/commit/d533dabfa709a27df9fcf1c34478361b01906400))
    - Use Mode from eh1 in FrameFormat ([`ab0bf51`](https://github.com/winksaville/rp-hal/commit/ab0bf515638f8b2e053aca75f0bf9d265ab7d532))
    - Update embedded-hal naming in spi.rs ([`0bdaacb`](https://github.com/winksaville/rp-hal/commit/0bdaacb976dda9de1a66fd3b0a1dbfac4e7cbee3))
    - Update readme ([`8e1fea9`](https://github.com/winksaville/rp-hal/commit/8e1fea96983d8fa12e7ff55ea5845fb17bf26871))
    - Rename embedded-hal-1 to embedded-hal ([`978299f`](https://github.com/winksaville/rp-hal/commit/978299f613db23d45cadd4ada757ad39be40a25b))
    - Rename legacy embedded-hal to embedded_hal_0_2 ([`61d6e7d`](https://github.com/winksaville/rp-hal/commit/61d6e7d352bcea818cc39ebca8d763ffdf248d86))
    - Cargo fmt ([`1d91b0a`](https://github.com/winksaville/rp-hal/commit/1d91b0a10b1079cec094718b8f2223a0a946751d))
    - Make embedded-hal 1.0.0 non-optional ([`7e7b4ea`](https://github.com/winksaville/rp-hal/commit/7e7b4ea3ffb8178bfde8c4ed2a51ac0da191f8c2))
    - Merge pull request #712 from jannic/report-break-condition ([`6b040de`](https://github.com/winksaville/rp-hal/commit/6b040de62cac996af4df3e1b3f91bc4bd5a9ffa9))
    - Merge pull request #751 from jannic/issue-749 ([`bbdc2e9`](https://github.com/winksaville/rp-hal/commit/bbdc2e95174a8d63a225d82ab9ff30b305f3c7d8))
    - Implement defmt formatting and Debug for clocks::InitError ([`da7392e`](https://github.com/winksaville/rp-hal/commit/da7392e0dde9eff6ee9e0137c8088a7e049e7b05))
    - Merge pull request #708 from jannic/checked-i2c-construction ([`6f6dc5d`](https://github.com/winksaville/rp-hal/commit/6f6dc5d8df8f35d8223b2d4e3ca52f23958be79f))
    - Rename unchecked constructors ([`a965f1c`](https://github.com/winksaville/rp-hal/commit/a965f1c22ce53472545aa9f1731aaf1955077e66))
    - Merge pull request #746 from jannic/xosc-startup-delay ([`20a5cbc`](https://github.com/winksaville/rp-hal/commit/20a5cbc6a04e3cf17d41790dbab2550e4001849e))
    - Set startup_delay_multiplier of XOSC to 64 ([`f4340cd`](https://github.com/winksaville/rp-hal/commit/f4340cd86020905b7f93fe39b2f5ee259a3d46cb))
    - Add startup_delay_multiplier parameter to xosc initialization ([`38f5963`](https://github.com/winksaville/rp-hal/commit/38f59636574c82404591ba177aa07fa3029d9384))
    - Merge pull request #744 from jannic/set_top ([`e7128c5`](https://github.com/winksaville/rp-hal/commit/e7128c521c21b2e6378c634929658ea244a0266b))
    - Set TOP to 0xfffe by default and fix get_max_duty ([`04ce6ab`](https://github.com/winksaville/rp-hal/commit/04ce6ab5dbce496f1696fc22096275cc06f3a2c9))
    - Merge pull request #743 from jannic/namespaced_features ([`88fba72`](https://github.com/winksaville/rp-hal/commit/88fba72944ab7dedf72d99d316f4532588f32e45))
    - Use namespaced (`dep:`) features for optional dependencies ([`edc676e`](https://github.com/winksaville/rp-hal/commit/edc676e65d565eb85480a77c7594e84d0f10f990))
    - Merge pull request #727 from Sympatron/main ([`9c4eea7`](https://github.com/winksaville/rp-hal/commit/9c4eea7eba2eedb48c306428b165cec51311166b))
    - Merge branch 'main' into main ([`ec24ff2`](https://github.com/winksaville/rp-hal/commit/ec24ff27e3aa561f77e62608f1039aa7e49654c9))
    - Merge pull request #730 from jannic/replace-asm-macros ([`7c9117c`](https://github.com/winksaville/rp-hal/commit/7c9117cd868d4d5a2858fd8fe6c50a10f4c9e242))
    - Merge pull request #736 from jannic/implement-SetDutyCycle ([`33772d3`](https://github.com/winksaville/rp-hal/commit/33772d3c5b38926c327e924cf294b85ff0670602))
    - Merge pull request #715 from jannic/change-default-shift-direction ([`78418de`](https://github.com/winksaville/rp-hal/commit/78418de94a312a263572e18e421dbe0d17fa9bbb))
    - Merge pull request #738 from ithinuel/add-missing-validfunction-dynfunction-impl ([`3969e41`](https://github.com/winksaville/rp-hal/commit/3969e4194fb1abeaa1c5a4e722987d584fbf27fd))
    - Add missing ValidFunction implementation for DynFunction. ([`a8f6b2f`](https://github.com/winksaville/rp-hal/commit/a8f6b2f62ac04adb7b00681284332d01b7abbbbc))
    - Simplify pwm_blink examples ([`2b535ec`](https://github.com/winksaville/rp-hal/commit/2b535eceb604ea23a893cbfe9f34fb2aa473e663))
    - Make import conditional to avoid unused import warning ([`8e074f3`](https://github.com/winksaville/rp-hal/commit/8e074f394c8be8626164a6b0d8e7a35d1d2d6f99))
    - Implement embedded_hal::pwm::SetDutyCycle of embedded-hal 1.0 ([`db8641e`](https://github.com/winksaville/rp-hal/commit/db8641e429833f4367ee5c3f2cab81de911b50ff))
    - Merge pull request #734 from jannic/eh-1.0-rc3 ([`935c92a`](https://github.com/winksaville/rp-hal/commit/935c92a55278da654e5af769a6e719bbbe89188b))
    - Add delay_ms() implementation for DelayNs trait ([`87e2fb6`](https://github.com/winksaville/rp-hal/commit/87e2fb645462265584331a11ef9e1944a4aadae1))
    - Fix compilation with MSRV ([`130c9eb`](https://github.com/winksaville/rp-hal/commit/130c9eb0823f00766ef0605b8eb12b43f23878fe))
    - Upgrade embedded-hal 1.0 dependency to 1.0.0-rc.3 ([`d1289bb`](https://github.com/winksaville/rp-hal/commit/d1289bb4d530352a7520eb56851e30a3f63e8b94))
    - Replace asm macros by rust macros ([`5ffb3dc`](https://github.com/winksaville/rp-hal/commit/5ffb3dc549b9d34703808c52ebe287b7646bbcee))
    - Make embedded-io dependency non-conditional ([`117a643`](https://github.com/winksaville/rp-hal/commit/117a64366e6397dbfd1cbd5f6b0af3be0002d0ef))
    - Merge pull request #725 from jnthbdn/fix_rtc_ownership ([`85474db`](https://github.com/winksaville/rp-hal/commit/85474dbe1b119f0e7372f075f989c8884b2930ec))
    - Implement embedded-io Read + Write for UartPeripheral ([`3fef962`](https://github.com/winksaville/rp-hal/commit/3fef96222043359d5320b44715b09bde1b85cd6b))
    - Add free function ([`39d3c8d`](https://github.com/winksaville/rp-hal/commit/39d3c8d9328da832f1348f1e14adea18c049cbad))
    - Add free function ([`9372dce`](https://github.com/winksaville/rp-hal/commit/9372dce9c8a7e73e996975360b7bcf35db9489e2))
    - Merge pull request #726 from ithinuel/add-defmt-format-to-i2c-peripheral-evt ([`28ec527`](https://github.com/winksaville/rp-hal/commit/28ec5271f83bcbcf2ecbb18bf4bd819b248f1594))
    - Add derive(defmt::Format) to i2c::peripheral::I2CEvent ([`9293511`](https://github.com/winksaville/rp-hal/commit/929351180673338f66c6125c5af9968c28c95bf6))
    - Add from_installed_program with correct shift direction ([`50583b2`](https://github.com/winksaville/rp-hal/commit/50583b2c9347254b5f04a2b676f88b3e7ee0c1ec))
    - Merge pull request #723 from redolution/pio-irq-zst ([`cfd6c12`](https://github.com/winksaville/rp-hal/commit/cfd6c128a1688186f419e3bd60ce469ddeb7fb47))
    - Merge pull request #676 from ithinuel/enable-rtc-irq ([`41b3e41`](https://github.com/winksaville/rp-hal/commit/41b3e41e1a16579a5a8a8b364858f31edaa84811))
    - Merge pull request #718 from jannic/rand-docs ([`9f8c3a6`](https://github.com/winksaville/rp-hal/commit/9f8c3a685ac88ce962ed762efd8659ae7dfbef7c))
    - Fix dangling link ([`df9d35b`](https://github.com/winksaville/rp-hal/commit/df9d35b6b28786cd4e71b3b772bdbe60a10aea6f))
    - Improve formatting ([`a3fcf14`](https://github.com/winksaville/rp-hal/commit/a3fcf144f85b9260954b8a94376365aed2a3ad28))
    - Add a short explanation on how to use RingOscillator as a random number source ([`e681478`](https://github.com/winksaville/rp-hal/commit/e681478943aa9acbccb4e22488be00fbd5a16b42))
    - Allow getting PIO IRQs by index ([`12f8484`](https://github.com/winksaville/rp-hal/commit/12f848406d9e13f21a3d63cdb3c34f32ff7aaeb6))
    - Merge pull request #716 from jannic/revert-705 ([`1406331`](https://github.com/winksaville/rp-hal/commit/14063315c9679132e940e64118f45a32ba119481))
    - Fix test case in doc comment ([`bb8a9fd`](https://github.com/winksaville/rp-hal/commit/bb8a9fd7cede768a8c11a316e505fe76be4929e5))
    - Ensure that i2c pins have PullUp activated ([`6c6158d`](https://github.com/winksaville/rp-hal/commit/6c6158dcb72211b2badf1830df9a98f49f1a4a5c))
    - Merge pull request #719 from SCingolani/main ([`aecf366`](https://github.com/winksaville/rp-hal/commit/aecf36607b41e299bcdc01d92846100cbf59a842))
    - Merge pull request #720 from jannic/i2c-pull-up ([`cb0d2e9`](https://github.com/winksaville/rp-hal/commit/cb0d2e9733b088d622a8ac0de47c795c5015a8ec))
    - Merge pull request #721 from jannic/rom-function-safety-comments ([`9e2bad8`](https://github.com/winksaville/rp-hal/commit/9e2bad84b60a579a785bcb55af202393fee5df5e))
    - Add safety comments to unsafe rom function ([`6cb7a11`](https://github.com/winksaville/rp-hal/commit/6cb7a115d29fe71ee2f084c87e4ff34e01f107bc))
    - Configure i2c pins with pull-up in rustdoc example ([`867c8e9`](https://github.com/winksaville/rp-hal/commit/867c8e9c2f67969eba1ec94e8f36a21c693d39e2))
    - Fix greedy rosc `dormant()` - thanks @ithinuel ([`1bde6fd`](https://github.com/winksaville/rp-hal/commit/1bde6fd11987966b99b7e5afabd81f9e60f7ee7f))
    - Apply suggestions from code review ([`020c5b1`](https://github.com/winksaville/rp-hal/commit/020c5b1bf6068a7ee7b533bd882694d2bad81a9d))
    - Merge pull request #584 from ithinuel/prepare-for-next-usb-device-release ([`c69f4ce`](https://github.com/winksaville/rp-hal/commit/c69f4ce250ab682ec6a31f609a5727f9b1635426))
    - Additional safety comments for rosc/xosc dormant() - thanks @jannic ([`01da9fd`](https://github.com/winksaville/rp-hal/commit/01da9fd7c1e8676c75f400de9f41c5597f2e4838))
    - Fix clippy warnings ([`f823a81`](https://github.com/winksaville/rp-hal/commit/f823a81aa8a54da70ac065436e4af684ec0b5045))
    - Format example to standard ([`1f92a95`](https://github.com/winksaville/rp-hal/commit/1f92a95bdcb534f703cb7434410443e6e7be029a))
    - Bump msrv to 1.65 ([`f600a25`](https://github.com/winksaville/rp-hal/commit/f600a25f9649559a24483b051d1c1caf3e58b646))
    - Update usb-device implementation. ([`0918d37`](https://github.com/winksaville/rp-hal/commit/0918d37820ee11d11279fc71f25207f3308b7c38))
    - Make `Spi::free` also free up the pins ([`bcb7683`](https://github.com/winksaville/rp-hal/commit/bcb7683512363d0bf17675217bbafe7b050b7dcb))
    - Merge pull request #717 from jannic/release-0.9.1 ([`7b04000`](https://github.com/winksaville/rp-hal/commit/7b040006aec29a5f94695cf117ac30acd558c35e))
    - Prepare release 0.9.1, update changelog ([`f9c1346`](https://github.com/winksaville/rp-hal/commit/f9c1346949dc7256ede46e30d45e282ed5dde99c))
    - Merge pull request #668 from jlpettersson/enable_multiple_pwm_slices_atomically ([`357f4d6`](https://github.com/winksaville/rp-hal/commit/357f4d60ab2c9983b0de4f12c39678c2bb52ead4))
    - Merge pull request #688 from jannic/change-pll-settings ([`8a68410`](https://github.com/winksaville/rp-hal/commit/8a684106f82e51d8ce72591c3ef67b647bda7df3))
    - Merge pull request #714 from jannic/comment-shift-direction ([`757a0b0`](https://github.com/winksaville/rp-hal/commit/757a0b0a31b1302f60a37d264e5a4da5c3c685ea))
    - Revert "Make i2c::controller pub again" ([`dc5525c`](https://github.com/winksaville/rp-hal/commit/dc5525cd8faa1a19f21a0eb950d56c9e118a5420))
    - Merge pull request #705 from jannic/v0.9-semver-compat ([`0046f4d`](https://github.com/winksaville/rp-hal/commit/0046f4dcada94d38a746e632feed5fc6247470e8))
    - Document default value for ShiftDirection ([`93b7106`](https://github.com/winksaville/rp-hal/commit/93b7106e0a29298a94f39e190d36acbaed2a0deb))
    - Improve handling of UART status bits ([`6a1a0a2`](https://github.com/winksaville/rp-hal/commit/6a1a0a2989d2961c8dabf3d24745c4d0b56094ac))
    - Merge pull request #713 from jannic/flush_should_check_busy ([`fbb7e79`](https://github.com/winksaville/rp-hal/commit/fbb7e79f254720c05bc654a7b0eb18f15f767263))
    - Fix UART transmit_flushed method ([`34200ed`](https://github.com/winksaville/rp-hal/commit/34200ed88e2a03bdd321bcf0535d5378e3492649))
    - Merge pull request #709 from jannic/improve-docs ([`a640cf0`](https://github.com/winksaville/rp-hal/commit/a640cf0105dc159d0e5319b712b82cc89ff06d04))
    - Fix typo ([`bd98b5f`](https://github.com/winksaville/rp-hal/commit/bd98b5feb0fc25f37d2be079dade786d639ef1f5))
    - Properly report break conditions ([`52279dc`](https://github.com/winksaville/rp-hal/commit/52279dc8d53688a3a47f05b735b7a940affc7cb5))
    - Merge pull request #711 from Rahix/uart-busy ([`e70ad80`](https://github.com/winksaville/rp-hal/commit/e70ad80541424e68809ffa9ea5a3dfea18a82e31))
    - Add uart_is_busy() method for UART devices ([`c4288dc`](https://github.com/winksaville/rp-hal/commit/c4288dcc66c5755523f76906eea48f2adc081f88))
    - Merge pull request #573 from jannic/issue-572 ([`b1542aa`](https://github.com/winksaville/rp-hal/commit/b1542aae56f51b774a3f270515c39a61e3446d3c))
    - Use fugit re-export in examples ([`799f9db`](https://github.com/winksaville/rp-hal/commit/799f9db27aeb9b4971f1a92ae954be6af9990115))
    - Hide re-export of paste crate from docs ([`111caaf`](https://github.com/winksaville/rp-hal/commit/111caaf61e05e9093de647cfe9cc4e14688b96a9))
    - Re-export fugit ([`a586a5d`](https://github.com/winksaville/rp-hal/commit/a586a5dc42d8ca80bf5b4995862f4f7be95d99d4))
    - Mention linker flags in README ([`dd5f479`](https://github.com/winksaville/rp-hal/commit/dd5f4796af36219494466241969cc4e6fcb7600b))
    - Merge pull request #670 from ThadHouse/flush_pio ([`e117359`](https://github.com/winksaville/rp-hal/commit/e11735983feeb6ab7509683edcb67f6d23054789))
    - Merge pull request #702 from ithinuel/improve-spi-peripheral-documentation ([`a5f0609`](https://github.com/winksaville/rp-hal/commit/a5f06090b1001a35c1b8ff54bd9f0ad8249abbdb))
    - Improve `Spi::new` documentation ([`50f6029`](https://github.com/winksaville/rp-hal/commit/50f60298456f007eea13e071c2441911321f4ace))
    - Merge pull request #699 from fu5ha/improve-spi-docs ([`5706ea2`](https://github.com/winksaville/rp-hal/commit/5706ea2f6a3575651caf72ac2b28e57938c219bf))
    - Make i2c::controller pub again ([`0e0506c`](https://github.com/winksaville/rp-hal/commit/0e0506ce94a5347c9972c72714953885108cea4b))
    - Fix module level doc example ([`661b98a`](https://github.com/winksaville/rp-hal/commit/661b98ac9c62d87a1a4fcef2f2ff1cc99639c1f8))
    - Fix order of function arguments in doc comment ([`2af733e`](https://github.com/winksaville/rp-hal/commit/2af733e1994ed14bdeb76111d3ace62b7144c52a))
    - Small tweak ([`b498c31`](https://github.com/winksaville/rp-hal/commit/b498c311b79eea39fa9d984bd7344523d5820875))
    - Improve Spi device/peripheral docs ([`d9f8ef4`](https://github.com/winksaville/rp-hal/commit/d9f8ef4823cea759e5d67b1f90282cf4a56b0b2e))
    - Merge pull request #704 from ithinuel/document-i2c-error-derives ([`14b6ee3`](https://github.com/winksaville/rp-hal/commit/14b6ee339345eb320bb047c635b6ae7ac8927124))
    - Document what's happening with derives on i2c::Error ([`51badca`](https://github.com/winksaville/rp-hal/commit/51badca0b4cc0dd3b06b89e07dfc743ea6c23bab))
    - Merge pull request #703 from rp-rs/add-i2c-iter ([`9c17a2d`](https://github.com/winksaville/rp-hal/commit/9c17a2db4dee73e407d16d283e6cb34b25b71ec9))
    - Implement WriteIter and WriteIterRead ([`001270f`](https://github.com/winksaville/rp-hal/commit/001270ff517bfdee3330a7ed118d98736f5526ed))
    - Incorporated feedback from @ithinuel ([`57c52db`](https://github.com/winksaville/rp-hal/commit/57c52db8e971f059be67838a1706b26ad833aa49))
    - Format to rust standard ([`0e4593b`](https://github.com/winksaville/rp-hal/commit/0e4593bf652a645f5fd448ca5c845e07ff512735))
    - DORMANT sleep example ([`a564d2e`](https://github.com/winksaville/rp-hal/commit/a564d2e28de5969e381ddb1e334b7eb6475064fd))
    - No need to switch a glitchless clock back to its default source first when changing to a non-aux source (e.g. reference clock changing to xosc). This allows us to turn off rosc if we want to. ([`be0f81a`](https://github.com/winksaville/rp-hal/commit/be0f81a8b1066a7a2bf52aa05800b3e6f2c8a824))
    - Allow running PLLs to be powered down, as needed for low-power DORMANT mode ([`c49fbb5`](https://github.com/winksaville/rp-hal/commit/c49fbb52f9e48fe5134a66803df47c374010b601))
    - Add [RX]OSC transitions from Dormant back to the relevant wakeup state ([`18a6429`](https://github.com/winksaville/rp-hal/commit/18a642918d339688fe6a12ac096d5fe6128639ed))
    - Merge pull request #698 from jannic/probe-rs-migration ([`c4fbc4b`](https://github.com/winksaville/rp-hal/commit/c4fbc4befa2763588939805addfd2b942accb64e))
    - Use probe-rs in on-target tests ([`6de15d5`](https://github.com/winksaville/rp-hal/commit/6de15d56df4050f84701fe23ca1c1df342bd4cc1))
    - Fix MSRV check by using older version of regex ([`e676ec5`](https://github.com/winksaville/rp-hal/commit/e676ec5a937c26819d61f37f67c801df06b4728f))
    - Replace probe-run by probe-rs ([`7b6a331`](https://github.com/winksaville/rp-hal/commit/7b6a3319b8476de3846112bcccd5c62f26f048ac))
    - Merge pull request #692 from ithinuel/improve-i2c-peripheral-documentation ([`9bde6b5`](https://github.com/winksaville/rp-hal/commit/9bde6b576ddf19d310e02e1f216b06f4924d6c45))
    - Merge pull request #697 from 9names/fix_spi_example_comments ([`0713409`](https://github.com/winksaville/rp-hal/commit/071340957bd8c1a57da0066219798342f3b3f9df))
    - Fix out-of-date comment about SPI pins ([`999b95c`](https://github.com/winksaville/rp-hal/commit/999b95c0931d7dbf7d29d4b9722995ce716e98e0))
    - Merge pull request #694 from jannic/issue-689-implement-input ([`d70164c`](https://github.com/winksaville/rp-hal/commit/d70164c41577a45b517654af27c2c8460a3c3a06))
    - Improve comment ([`ec1b013`](https://github.com/winksaville/rp-hal/commit/ec1b0136ffbbf957fe490a3701397105f7b81f17))
    - Merge pull request #695 from jannic/rename_inner_read ([`fcebdea`](https://github.com/winksaville/rp-hal/commit/fcebdea7fd331c7d690bb97d9679fab3277507f4))
    - Rename private function Adc::read to Adc::inner_read ([`5442656`](https://github.com/winksaville/rp-hal/commit/54426566079be3335e5d7629de6f95a66170c1f6))
    - Merge pull request #677 from jannic/fix-future-clippy-warnings ([`43ddad5`](https://github.com/winksaville/rp-hal/commit/43ddad565ce5c4f3a93a8ed1f3a4e54e556a5943))
    - Disable clippy lint needless_pass_by_ref_mut ([`1d76507`](https://github.com/winksaville/rp-hal/commit/1d765071a427c83327a99470b7c28624a94d3c42))
    - Remove eh 1.0 implementation of InputPin for pin in mode SioOutput ([`59dcb38`](https://github.com/winksaville/rp-hal/commit/59dcb384dffc62ec280f7e75751b7232dd8a5d2d))
    - Implement InputPin for all pin configurations ([`6c24b50`](https://github.com/winksaville/rp-hal/commit/6c24b50e71c16b623c6f9448394dcceaeb26ac99))
    - Improve documentation of the i2c peripheral driver & improve i2c example ([`f87438b`](https://github.com/winksaville/rp-hal/commit/f87438b1a2a3521138596fbcb1c284bcedc51aeb))
    - Merge pull request #691 from vinsynth/feature/fix-refdiv ([`c47cb04`](https://github.com/winksaville/rp-hal/commit/c47cb04d58a0574ba7e30090598b79f211f7fd94))
    - Run 'cargo fmt' ([`b0b471c`](https://github.com/winksaville/rp-hal/commit/b0b471c6e396269a39ca0d5725a603a74ae0cb67))
    - Removed second division by `refdiv` ([`4142678`](https://github.com/winksaville/rp-hal/commit/4142678065049d652962c2349318e6fb80246e86))
    - Update CHANGELOG ([`2b758cf`](https://github.com/winksaville/rp-hal/commit/2b758cf8b119e6b7e4285e2167311dced9625841))
    - Use same USB_PLL default setting as the C SDK ([`efdee29`](https://github.com/winksaville/rp-hal/commit/efdee29cf07f30d477fda055aac02726b17001c6))
    - Merge pull request #685 from jannic/scratch-registers ([`78f71ae`](https://github.com/winksaville/rp-hal/commit/78f71ae2f12d67af07c79277461ec6e7606e3267))
    - Merge pull request #613 from jannic/issue-564 ([`2eb3d6f`](https://github.com/winksaville/rp-hal/commit/2eb3d6f24d9f16d2ecc2f50c1ac87914e144a0c8))
    - Use match instead of if/else ([`1aec0cb`](https://github.com/winksaville/rp-hal/commit/1aec0cba0cd0b0caad511a6632c87d73e36a72db))
    - Do a full reset, even though it breaks an open debug connection ([`adfa1a2`](https://github.com/winksaville/rp-hal/commit/adfa1a236be38246d1b699310a585ef4414123be))
    - Adapt to changes from #585 ([`5b6afe1`](https://github.com/winksaville/rp-hal/commit/5b6afe15a193f1aee87b1843ac25a4242fc32123))
    - Implement reset() and halt() functions ([`e82ecea`](https://github.com/winksaville/rp-hal/commit/e82eceab23a7cfb12debbc3f875b03650daa0925))
    - Use an enum instead of a numeric value to select scratch register ([`bc71bd9`](https://github.com/winksaville/rp-hal/commit/bc71bd92926f784aedd1d474d089b9021d02c142))
    - Provide functions to access watchdog scratch registers ([`11d02f4`](https://github.com/winksaville/rp-hal/commit/11d02f4bb2988f65dd5a185306473376baf4e03b))
    - Merge pull request #681 from ithinuel/migrate-to-eh10rc ([`6756d35`](https://github.com/winksaville/rp-hal/commit/6756d355659739226d7135f6b6dce63b92070c9f))
    - Update README regarding embedded-hal support preview ([`f62f19c`](https://github.com/winksaville/rp-hal/commit/f62f19c03b74c5fed556665da09a57b33484e653))
    - Remove spurious delay in rtc_example & fix doc on rtc::clear_interrupt ([`038f4ba`](https://github.com/winksaville/rp-hal/commit/038f4baab6a0307a360758b311d96858907c17d7))
    - Migrate to eh1_0 rc 1 ([`c2bd426`](https://github.com/winksaville/rp-hal/commit/c2bd426be66ebc4411b395ee0c77e6533f16e68e))
    - Merge pull request #663 from jannic/update-changelog ([`8f3e8d0`](https://github.com/winksaville/rp-hal/commit/8f3e8d0f61415297f0f26db80b2ed84ccea64317))
    - Define proper bitfields for clock gates' controlers ([`78e79ae`](https://github.com/winksaville/rp-hal/commit/78e79ae837e97192fb8082e32d638ddb71116b96))
    - Add some more CHANGELOG entries ([`c09d87a`](https://github.com/winksaville/rp-hal/commit/c09d87aa96370d3c71e4ee1379655313e4e638c9))
    - Skip alpha release - next version will be 0.9.0 ([`7e7cc9d`](https://github.com/winksaville/rp-hal/commit/7e7cc9d430378da82f0ffda44ab0965942590e23))
    - Update version number in README ([`75ff8da`](https://github.com/winksaville/rp-hal/commit/75ff8daadf5c865809d9f45000e7a3d926fe01ef))
    - Update CHANGELOG.md ([`c63132b`](https://github.com/winksaville/rp-hal/commit/c63132b5df876332964396d5500e7d019948d382))
    - Merge pull request #680 from jannic/fix-build-errors ([`cff601f`](https://github.com/winksaville/rp-hal/commit/cff601f9a2975329115ee548ec78c9ad69c06561))
    - Merge pull request #679 from agausmann/patch-1 ([`6f1c3cc`](https://github.com/winksaville/rp-hal/commit/6f1c3cc39bd93e7a4e29c120c134aada77291858))
    - Fix build errors introduced by #621 ([`82aab64`](https://github.com/winksaville/rp-hal/commit/82aab646dba83bf224f74480e28aff41de119459))
    - Merge pull request #621 from jannic/unsafe-dma-targets ([`d46bb60`](https://github.com/winksaville/rp-hal/commit/d46bb60ed4beec55504b0ffe6c6f3a2fb8cffbec))
    - Document limitations of I2C hardware ([`d5371de`](https://github.com/winksaville/rp-hal/commit/d5371de4134c72e2939c2fc77415c48a7efc5ea0))
    - Enhance rtc examples inline documentation ([`066371d`](https://github.com/winksaville/rp-hal/commit/066371da1630577822b38b4fb9933b03eb640f7b))
    - Update chrono integration ([`ff0f6ed`](https://github.com/winksaville/rp-hal/commit/ff0f6eda5ef28c62e317131bbe51b2c6c5dee864))
    - Add rtc_sleep_example and `ClockManager::configure_sleep_en` ([`1493989`](https://github.com/winksaville/rp-hal/commit/1493989a4559a6037511e0da8f40313be810033a))
    - Add rtc_irq_example ([`0a4b7d3`](https://github.com/winksaville/rp-hal/commit/0a4b7d32d0055eea1eef40df7f82ce6b0497f5dc))
    - Merge pull request #675 from jlpettersson/fix_typo ([`a12bcda`](https://github.com/winksaville/rp-hal/commit/a12bcdae6effc8d9fe58d5de3c8edf67f23fe529))
    - Fix typo ([`b34ae51`](https://github.com/winksaville/rp-hal/commit/b34ae518c2b4016c69f4aae3bce14ae4e32d2216))
    - Merge pull request #674 from jannic/bump-msrv ([`0a543d8`](https://github.com/winksaville/rp-hal/commit/0a543d87b3b03c8ca0aed08986819c88bde3d871))
    - Bump MSRV to 1.64 ([`6bf37e7`](https://github.com/winksaville/rp-hal/commit/6bf37e7782a54cdaf17fa41b788ed2b391292817))
    - Add function to clear PIO fifos ([`ff3c9a6`](https://github.com/winksaville/rp-hal/commit/ff3c9a630295f010d10eb62d0d989c77fe20c3e6))
    - Add function to enable multiple PWM slices at the same time ([`a7f51b7`](https://github.com/winksaville/rp-hal/commit/a7f51b7d902ccac0b59cc320e49ed95ddadd8c81))
    - Merge pull request #654 from NelsonAPenn/feature/spi_frame_format ([`76efb36`](https://github.com/winksaville/rp-hal/commit/76efb36f7d54b04246c3f8c68cbfa12612f5f09e))
    - Merge pull request #666 from jannic/lock-cargo-hack-version ([`6508033`](https://github.com/winksaville/rp-hal/commit/6508033b0cbc561dc399463ed902efa4395c2215))
    - Fix version of cargo-hack to 0.5.28 ([`e16c596`](https://github.com/winksaville/rp-hal/commit/e16c596f6711e154eb171ae7da228905ca0fad52))
    - Run cargo fmt ([`a701dd8`](https://github.com/winksaville/rp-hal/commit/a701dd8aef2982ab7583b05ed24de384c4b4b0c4))
    - Merge pull request #664 from jannic/fix-doc-test ([`c1f6c1c`](https://github.com/winksaville/rp-hal/commit/c1f6c1c9261e180570cc983de6189e349655292f))
    - Fix an import in a doc comment ([`374d1f0`](https://github.com/winksaville/rp-hal/commit/374d1f03ed5c19c843172aa3728a2a6c17b4dc57))
    - Merge pull request #662 from jannic/pac-0.5.0 ([`cf0a1ca`](https://github.com/winksaville/rp-hal/commit/cf0a1ca3e647b857521606196bd36cf4010d598e))
    - Don't try to enable feature critical-section-impl on rp2040-hal-macros ([`fce2106`](https://github.com/winksaville/rp-hal/commit/fce2106a69ba120287ff91b245adec1ffca5efa3))
    - Minor cosmetic fix ([`cde4601`](https://github.com/winksaville/rp-hal/commit/cde46017efc69682718317b6e92d138623f94349))
    - Activate feature critical-section-impl for tests ([`a805df1`](https://github.com/winksaville/rp-hal/commit/a805df14936ef81adeb3c3b5ddae0750eacd6598))
    - Changes necessary for updated PAC ([`194577f`](https://github.com/winksaville/rp-hal/commit/194577fe065b28bebb3392c9374a8575d805d4cc))
    - Update rp2040-pac to version 0.5.0 ([`a19ddfd`](https://github.com/winksaville/rp-hal/commit/a19ddfd8ae741359e8624cbe69d996e82b540be8))
    - Merge pull request #661 from Tomin1/correct_pio_irq_doc ([`49c27c2`](https://github.com/winksaville/rp-hal/commit/49c27c25d5e5feb2ad83751b908897df61a3ebea))
    - Correct PIO::irq[01] documentation ([`82fd22b`](https://github.com/winksaville/rp-hal/commit/82fd22b23d8ca83c021dfb947511ef8fc1ce87f3))
    - Add derive macros ([`4d0ffd1`](https://github.com/winksaville/rp-hal/commit/4d0ffd1433e189757ac8e0fb1a66ffbba1fd4ac8))
    - Remove spi::Mode, impl Into for FrameFormat ([`f519e0d`](https://github.com/winksaville/rp-hal/commit/f519e0dd90da64575b20cad6fddf9c578973e3e6))
    - Merge pull request #645 from jannic/use-fixed-nightly-version-for-udeps ([`0633232`](https://github.com/winksaville/rp-hal/commit/0633232089170c48bb454e854cf488d1f3ae85bf))
    - Merge pull request #651 from ithinuel/migrate-to-edition-2021 ([`d9231cf`](https://github.com/winksaville/rp-hal/commit/d9231cf64fb1898a6efec317564c6e797c51b016))
    - Merge pull request #655 from ithinuel/fix-uart-debug-add-defmt ([`6600e44`](https://github.com/winksaville/rp-hal/commit/6600e4477ec6341ef12cc85247b8916068455d0d))
    - Add defmt::Format to serial read & always derive Debug ([`5b57ba8`](https://github.com/winksaville/rp-hal/commit/5b57ba8b4b091f8f54c8cb1c5b363a0ea4ba1f1b))
    - Make doc exampe use new init interface ([`9596512`](https://github.com/winksaville/rp-hal/commit/9596512e6eab39c22aa2eeda4070da42ee5577cf))
    - Merge pull request #640 from hardiesoft/feature/init_rosc_with_known_frequency ([`3b5bbfb`](https://github.com/winksaville/rp-hal/commit/3b5bbfbe749228428ab5d729bbc43ffc7167aa84))
    - Update broken examples; clippy ([`0c2f99d`](https://github.com/winksaville/rp-hal/commit/0c2f99d568f258115940f307f643da0e9d189356))
    - Remove unused Into<Mode> generic ([`f042839`](https://github.com/winksaville/rp-hal/commit/f04283954e73f25e0e90752bf33d4d0cd760a751))
    - [spi] Make SPI set_format accept frame format ([`e84c296`](https://github.com/winksaville/rp-hal/commit/e84c29623726a411168d0a79bde57ef0e8f15f15))
    - Merge pull request #653 from jannic/issue-641 ([`8a0b9fc`](https://github.com/winksaville/rp-hal/commit/8a0b9fc8a700c128b53a97ea99c9513bf7f05422))
    - Address rustfmt and clippy warnings. ([`178854e`](https://github.com/winksaville/rp-hal/commit/178854ea2f862b452001b3af354c71ac8dc1ec82))
    - Fix calculation of MPU RBAR value ([`ff8f8fe`](https://github.com/winksaville/rp-hal/commit/ff8f8fec2d2cb60db767920781445a93b039034e))
    - Merge pull request #649 from adrianparvino/usb ([`c8935b0`](https://github.com/winksaville/rp-hal/commit/c8935b084d7677f4fbaef0600927a809714db474))
    - Fix lifetimes and mutability of `get_buf` and `get_buf_mut` ([`d8b48c6`](https://github.com/winksaville/rp-hal/commit/d8b48c6e190ef65fe1a4cce702b1dcaf6aa37f5a))
    - Address review feedback and add an example of setting ROSC to a desired frequency (2). ([`1a6b425`](https://github.com/winksaville/rp-hal/commit/1a6b4256db0cd48ba702def43b8df95d6d5b60fd))
    - Address review feedback and add an example of setting ROSC to a desired frequency. ([`b5e2be8`](https://github.com/winksaville/rp-hal/commit/b5e2be856c9ecd8fa5caa02fe59e91556426168d))
    - Migrate rp2040-hal to edition 2021 ([`c4d3fa8`](https://github.com/winksaville/rp-hal/commit/c4d3fa882acc5b19269d20ff74f65f1e53e81ee9))
    - Merge pull request #648 from nilclass/rename-dma-channel-listen ([`c7e6cca`](https://github.com/winksaville/rp-hal/commit/c7e6ccaf18670c81087d04563a9907aa2eaf3a14))
    - Merge pull request #571 from jannic/syn2 ([`a11741d`](https://github.com/winksaville/rp-hal/commit/a11741d8cce4bea7c00d696174aeafbcfad25aff))
    - Merge pull request #646 from mBornand/pwm_writetarget ([`14a9549`](https://github.com/winksaville/rp-hal/commit/14a95499a646337216169e828edcb8de52fcce45))
    - Update comment in example ([`4f3e7d8`](https://github.com/winksaville/rp-hal/commit/4f3e7d855e0d8d0af1b58f7f2b2eafebe2b217e4))
    - Rename `dma::SingleChannel::listen_irq*` to `enable_irq*` ([`da99eeb`](https://github.com/winksaville/rp-hal/commit/da99eeb6711d7ac671ff720bbdfc87f37c9f08ea))
    - Merge pull request #636 from nilclass/adc-fifo-dma ([`f324a30`](https://github.com/winksaville/rp-hal/commit/f324a30a7a1bebed751bf36da0ac90607bf88ee2))
    - Merge pull request #647 from jannic/avoid-missing-doc-warning ([`df8e614`](https://github.com/winksaville/rp-hal/commit/df8e614799c0480041ad0e81ed2e059c62b45881))
    - Avoid missing docs warning on pub extern crate ([`b10372d`](https://github.com/winksaville/rp-hal/commit/b10372d4b9fe4ef322987caf32c8d7df3f6fbcfe))
    - Fix typo and manually implement PartialEq ([`d10d449`](https://github.com/winksaville/rp-hal/commit/d10d449a03eee50ebf5ede3c9b89889500e284c7))
    - Stop writting to the upper TOP register ([`4d62fd0`](https://github.com/winksaville/rp-hal/commit/4d62fd0e2ae0a9b5c75b714fbab5886cce1a44d7))
    - Update rp2040-hal/src/pwm/mod.rs ([`6ff3b88`](https://github.com/winksaville/rp-hal/commit/6ff3b886b9b116804a604615e7cefb2c583bb30a))
    - Implement WriteTarget for PWM top and cc registers. ([`f2910d3`](https://github.com/winksaville/rp-hal/commit/f2910d3299c2cbcac942252e16512aac0eb00dfc))
    - Also pin cargo-udeps to version 0.1.40 ([`8aa3e81`](https://github.com/winksaville/rp-hal/commit/8aa3e81a8e8b16a46b152effa5db7fa07f0ca40c))
    - Use fixed version nightly-2023-06-27 for cargo udeps ([`10e80e0`](https://github.com/winksaville/rp-hal/commit/10e80e011c2bc1207dea338c4483fa95c46abc29))
    - Fix a typo ([`172b1fa`](https://github.com/winksaville/rp-hal/commit/172b1fab437670fe2bf1341d25373a27eeb315d2))
    - Merge pull request #642 from jannic/eh-1-0-0-alpha-11 ([`6c74c62`](https://github.com/winksaville/rp-hal/commit/6c74c62d0144d5931b7fd53b0900290122c4b19c))
    - Merge pull request #623 from jannic/alpha ([`17aa070`](https://github.com/winksaville/rp-hal/commit/17aa0704ae6444ab8f115a77f2dd42357b9293df))
    - Typo, clarification ([`0f9f891`](https://github.com/winksaville/rp-hal/commit/0f9f891a5126eb2c9ffde78a1dc0982460ad23f1))
    - Fix doc example, so it compiles ([`852e090`](https://github.com/winksaville/rp-hal/commit/852e0902aeb1ec3dfb9f5ebf199ddb28728c0edd))
    - Mention DMA example in docs ([`e0649d0`](https://github.com/winksaville/rp-hal/commit/e0649d092a0ab4e1331fe13cc88e469c336622c2))
    - Tweak example ([`2a896d5`](https://github.com/winksaville/rp-hal/commit/2a896d5f327d483e75311102043f2d0fdf6f661f))
    - Fmt, clippy ([`b06fe1a`](https://github.com/winksaville/rp-hal/commit/b06fe1a39c4f41a9f25dea3a4ff6f6d19a7e34a6))
    - Merge pull request #602 from jannic/build-tests ([`8962048`](https://github.com/winksaville/rp-hal/commit/8962048d43971f4cd78444463aa8ad94a4863092))
    - Remove `start_dma` in favor of `enable_dma` / `prepare` ([`f79d6dd`](https://github.com/winksaville/rp-hal/commit/f79d6ddfe30019e11aa7ccfda59c44a6221b2480))
    - Add `start_dma` method to `AdcFifoBuilder` ([`b7cffdb`](https://github.com/winksaville/rp-hal/commit/b7cffdb209f40124740fa872027b01263b141949))
    - Update to embedded-hal 1.0.0-alpha.11 ([`b5930a2`](https://github.com/winksaville/rp-hal/commit/b5930a27353a89383815761c316ad6ba15e1d62a))
    - Merge pull request #609 from tomgilligan/main ([`3b2738a`](https://github.com/winksaville/rp-hal/commit/3b2738ac2cb4980b13ab06654696c7de518c0980))
    - Merge pull request #644 from jannic/bump-msrv ([`f95393a`](https://github.com/winksaville/rp-hal/commit/f95393a486525291345983a85557bd20bd6bfb8e))
    - Bump MSRV to 1.63 ([`cb5ab33`](https://github.com/winksaville/rp-hal/commit/cb5ab338224e3d40b73d2e77cb4759418397100c))
    - Adds the ability to initialise the ring oscillator with a known frequency.  This PR is necessary because freq_hz is a private member of the `RingOscillator<Enabled>` struct. ([`6246a0b`](https://github.com/winksaville/rp-hal/commit/6246a0be676a6d73080057b8ddab5446968afd06))
    - Merge pull request #639 from mrdxxm/usb-set-device-patch ([`b1eea90`](https://github.com/winksaville/rp-hal/commit/b1eea90ebe779409ea63ccb21291c11f8b684561))
    - Fix of usb device address mask ([`59ceb47`](https://github.com/winksaville/rp-hal/commit/59ceb477d5adf64ab1a55b9f83519369ce6670ae))
    - Merge pull request #626 from nilclass/free-running-adc ([`08f5e0f`](https://github.com/winksaville/rp-hal/commit/08f5e0f88b0734f93a3a11c172e566f571863dc2))
    - Clippy adjustments for examples ([`dc5901c`](https://github.com/winksaville/rp-hal/commit/dc5901cbc8ff7d78b41e1d9abe3d656cfe76cd8d))
    - Use `ignore` for doc comments that can't compile ([`fe5023f`](https://github.com/winksaville/rp-hal/commit/fe5023f56eb39bd223b0944d08f6cac88e866d53))
    - Adjust documentation, mark code blocks properly ([`708a511`](https://github.com/winksaville/rp-hal/commit/708a511046eb6439cc623ae861e457de71c16714))
    - Formatting & clippy ([`a272084`](https://github.com/winksaville/rp-hal/commit/a272084207532737136737fa8156b5f06299b138))
    - Merge pull request #633 from schanur/patch-1 ([`ed8fd5b`](https://github.com/winksaville/rp-hal/commit/ed8fd5b003b71a16fba538ce326de6959aa127b2))
    - Add `read_single` to `AdcFifo` ([`ba68bfe`](https://github.com/winksaville/rp-hal/commit/ba68bfedca55e6e19d94de9a4ab0322a50f2ec6d))
    - Document `AdcFifoBuilder.clock_divider` ([`0ed047c`](https://github.com/winksaville/rp-hal/commit/0ed047c4675a35b854d605d39f75ed25c997ceb5))
    - Wait for CS.READY before draining fifo ([`70ea42c`](https://github.com/winksaville/rp-hal/commit/70ea42c4c6581219f3c5bb75ef906d6d2879f9f3))
    - Fixed wrong comment in pwm_irq_input.rs ([`44c60ab`](https://github.com/winksaville/rp-hal/commit/44c60ab85d46e6b631cbc3b4bf21e71bb1be1528))
    - Merge pull request #632 from Momijiichigo/patch-1 ([`882dead`](https://github.com/winksaville/rp-hal/commit/882deada4ec0a17d929a5b714d2d874fe94bf597))
    - Fix datasheet section number ([`bacd978`](https://github.com/winksaville/rp-hal/commit/bacd978f4bd9a66c46f4a6c0b020ea306f7ff1c3))
    - Update examples after rebase ([`bc53742`](https://github.com/winksaville/rp-hal/commit/bc537425e6cc860bd63b264a109da05e93c6e339))
    - Add `AdcFifoBuilder::shift_8bit` method ([`89d50f9`](https://github.com/winksaville/rp-hal/commit/89d50f9b31e9eb328e39331ec5ab29511c8af307))
    - Add example: adc_fifo_irq ([`85a5c4b`](https://github.com/winksaville/rp-hal/commit/85a5c4b3fdcb3eaeb78afa79dcb7271a0ac686f8))
    - Drain remaining values from FIFO, to prevent interrupts ([`0129221`](https://github.com/winksaville/rp-hal/commit/01292212779342c860163a9a7e6d6481c828e1ad))
    - Doc fixes ([`2cf81e9`](https://github.com/winksaville/rp-hal/commit/2cf81e97c5c3372b699f45cfb2c9b2648603f749))
    - Remove unused "num-traits" dependency ([`a2541fe`](https://github.com/winksaville/rp-hal/commit/a2541fe672db34f455f4a240c80f9f062cf8a2e4))
    - Add example: adc_fifo_poll ([`c45dac0`](https://github.com/winksaville/rp-hal/commit/c45dac093981060de3fa02b8c8cf6be5d55af2c0))
    - A bit of renaming; remove DMA related code ([`9a96526`](https://github.com/winksaville/rp-hal/commit/9a96526bf56f01ce1a12e7a5b70de66218657236))
    - Free-running mode experiments ([`63c761d`](https://github.com/winksaville/rp-hal/commit/63c761d0b58b3150c1533aa31a343a3f8c429694))
    - Merge pull request #631 from jannic/adc-field-names ([`dc7b8ca`](https://github.com/winksaville/rp-hal/commit/dc7b8caa1f3c145692b6695f041f85ae11dd3619))
    - Rename field names of struct AdcPin ([`3ee18b6`](https://github.com/winksaville/rp-hal/commit/3ee18b6efd0fdea5013ed79758d6a2049c65cb04))
    - Merge pull request #629 from jannic/issue-628 ([`fe3a881`](https://github.com/winksaville/rp-hal/commit/fe3a881b37f5d670e80e9a9b2e7c2e37a67c41cf))
    - Fix URL of pico_usb_serial example ([`79cfaac`](https://github.com/winksaville/rp-hal/commit/79cfaac3d14f1d81556406822bcaa18f277be41a))
    - Merge pull request #627 from pietgeursen/patch-1 ([`2698ce7`](https://github.com/winksaville/rp-hal/commit/2698ce79684f927bb72e40975fb41f725c7d3ff8))
    - Fix typo in `impl_write!` call. 22 should be 12 ([`ad8eb13`](https://github.com/winksaville/rp-hal/commit/ad8eb138f34174af01890397bdcc0efc27e241b7))
    - Merge pull request #622 from jannic/clippy-warning ([`6496c26`](https://github.com/winksaville/rp-hal/commit/6496c26dd7d7908a6d2e9531275c110aa921e4fb))
    - Add safety comments ([`4976e93`](https://github.com/winksaville/rp-hal/commit/4976e9300202bb4b7b4571d848d7c065c6aef162))
    - Mark ReadTarget and WriteTarget as unsafe ([`e22c5c0`](https://github.com/winksaville/rp-hal/commit/e22c5c013347eb09d585710abb9f96e060448dba))
    - Merge pull request #624 from jannic/on-target-tests ([`0b16b13`](https://github.com/winksaville/rp-hal/commit/0b16b136703ab75012e48cc9a72fe0ab6559115a))
    - Fix gpio configuration in on-target-tests ([`edad1d2`](https://github.com/winksaville/rp-hal/commit/edad1d2a2e48c41de09839982daa27ce6d20b253))
    - Don't specify version of rp2040-hal for on-target tests ([`45d4a21`](https://github.com/winksaville/rp-hal/commit/45d4a21c5167d411b9f992f7319996649fbe407f))
    - Fix gpio configuration in on-target-tests ([`0f5e77a`](https://github.com/winksaville/rp-hal/commit/0f5e77aa5eda5fabaf1ee3335b83815d8cf0e422))
    - Don't specify version of rp2040-hal for on-target tests ([`e2c749b`](https://github.com/winksaville/rp-hal/commit/e2c749b67db5e2bc10c11014bfeb9e5d277180ec))
    - Run clippy in CI with --all-features flag ([`6e0be27`](https://github.com/winksaville/rp-hal/commit/6e0be27f14b92001daffacc8da45bc4b62287455))
    - Disable a clippy warnining showing up with --all-features ([`bf82ab7`](https://github.com/winksaville/rp-hal/commit/bf82ab7c7f2dd000dc1503169c1f49f03ad6e241))
    - Prepare alpha release 0.9.0-alpha.1 ([`b26d8cf`](https://github.com/winksaville/rp-hal/commit/b26d8cf019c073c050492a71ca76b6da4a09cb55))
    - Merge pull request #617 from jannic/fix-changelog ([`7d49c2e`](https://github.com/winksaville/rp-hal/commit/7d49c2e3caed30533478830f3fa974c73294edc0))
    - Add several changelog entries ([`093c470`](https://github.com/winksaville/rp-hal/commit/093c4701cb0de6c69ccb21e0a09cbc50bf6a116c))
    - Merge pull request #618 from jannic/timer-needs-clocks ([`4f97282`](https://github.com/winksaville/rp-hal/commit/4f97282736b447551233291d6675c3d54c3710fc))
    - Update examples and doc comments ([`c9244f1`](https://github.com/winksaville/rp-hal/commit/c9244f115cb212f1198e86a2435b360c7ef62c4b))
    - Make sure clocks are initialized before creating a Timer ([`3788ed8`](https://github.com/winksaville/rp-hal/commit/3788ed8d705b3b2a5b156530706a41360714b42a))
    - Merge pull request #619 from ithinuel/bump-hal-to-0.9 ([`c9ffba0`](https://github.com/winksaville/rp-hal/commit/c9ffba0813f3790d2ba637138b88e079614f1ca8))
    - Bump hal's version ([`b4535ba`](https://github.com/winksaville/rp-hal/commit/b4535babbd7ba03ec89cdd25288f28f8698b45f5))
    - Merge pull request #598 from jannic/update-boot2 ([`6518dc5`](https://github.com/winksaville/rp-hal/commit/6518dc50d457afbd597ab6e4acbebe6dd4244f59))
    - Upgrade boot2 to version 0.3.0 ([`e3767cb`](https://github.com/winksaville/rp-hal/commit/e3767cbc1d4607b8e1118d115aca97b93204d747))
    - Merge pull request #594 from ithinuel/do-not-require-multicore-callback-to-never-return ([`4ab43cb`](https://github.com/winksaville/rp-hal/commit/4ab43cbf9687459f9c05fdda809f3946418f6620))
    - Merge pull request #616 from jannic/mode-from-reference ([`61eb7a1`](https://github.com/winksaville/rp-hal/commit/61eb7a17ea209c2c126b20c367305f5db50b95e9))
    - Update rp2040-hal/src/multicore.rs ([`6d55c14`](https://github.com/winksaville/rp-hal/commit/6d55c1452dd85f5d79b3504f875d4d4ac0da54f7))
    - Minor usability improvement ([`2dd37fe`](https://github.com/winksaville/rp-hal/commit/2dd37feb47e5af8afaddfd2d31821f47115624b4))
    - Merge pull request #614 from jannic/cloneable-timer ([`49d0460`](https://github.com/winksaville/rp-hal/commit/49d0460fc9ff188041695f253b6d925a60aa9623))
    - Merge pull request #607 from ithinuel/improve-errata5-documentation ([`cbf5fe6`](https://github.com/winksaville/rp-hal/commit/cbf5fe65c0672f87f989c97261da3edc8d5f1169))
    - Remove delay implementations with u64 parameters ([`7fb1484`](https://github.com/winksaville/rp-hal/commit/7fb1484cdf19110247c378398224e3dd54109448))
    - Rename internal delay function ([`e9aee64`](https://github.com/winksaville/rp-hal/commit/e9aee649123a8f931e73d7f09e9f30e6fe6c1b0e))
    - Fix comparison with u32::MAX for smaller types ([`ae9e1f5`](https://github.com/winksaville/rp-hal/commit/ae9e1f5f0793b0df26665bbfb8fb43d65f44d027))
    - Fix clippy warning ([`cd258f9`](https://github.com/winksaville/rp-hal/commit/cd258f9e87fcd6e55b0b80357bc185d5b198a994))
    - Implement delay using 32bit arithmetic ([`6aef40d`](https://github.com/winksaville/rp-hal/commit/6aef40d957c6925e8039a97c50c7d0e0868297c1))
    - Remove implementation details from doc comment ([`f69319b`](https://github.com/winksaville/rp-hal/commit/f69319b5bc5722e4cc30c938064bbb72274d32ae))
    - Implement DelayUs<T>, DelayMs<T> for more values of T ([`25dfeb8`](https://github.com/winksaville/rp-hal/commit/25dfeb8729049bc2966e126fc19b512ef1cec4e1))
    - Inline the three calls to timer() ([`291baa3`](https://github.com/winksaville/rp-hal/commit/291baa3958e826078399ce6a824d8fd0faee58cf))
    - Update blinky example ([`a9e88b1`](https://github.com/winksaville/rp-hal/commit/a9e88b1adec31e2f93e76783b4e693ca4e6343ee))
    - Make Timer cloneable ([`837486d`](https://github.com/winksaville/rp-hal/commit/837486dfb0cd8f63563151b50287a1af8496dc8b))
    - Merge pull request #612 from ithinuel/fix-ub-in-multicore ([`8b37ffe`](https://github.com/winksaville/rp-hal/commit/8b37ffe3d5003c710a2417c2628b9ed942fe78db))
    - Rename stack bottom to stack limit and fix misspelled misalignment ([`76ad39e`](https://github.com/winksaville/rp-hal/commit/76ad39eab93f3ea74869e65a4ef2e3ffe4673fa3))
    - Fix undefined behaviour in multicore ([`79fac38`](https://github.com/winksaville/rp-hal/commit/79fac385f47878e98343868c763b0b599958ffed))
    - Merge pull request #611 from tomgilligan/fix-alpha-spi ([`c5ea6d5`](https://github.com/winksaville/rp-hal/commit/c5ea6d56c38158f35116d6b32c74f2020669c724))
    - Remove redundant let ([`bc9784a`](https://github.com/winksaville/rp-hal/commit/bc9784a487e5654ccefcb73b3a80ca258930657e))
    - Simplify some types aroud Mode ([`ba0a5fa`](https://github.com/winksaville/rp-hal/commit/ba0a5fa6c8124b193dd97b71547b5b8fd7306579))
    - Pass Spi's Mode by value ([`94d724e`](https://github.com/winksaville/rp-hal/commit/94d724e9edc6a9ce0e6bdcd8c6d370fedd4892cb))
    - Reduce visibility of inner EH ([`62343a1`](https://github.com/winksaville/rp-hal/commit/62343a1a689cfeff4c78f5d725832604731883a3))
    - Use newtype to reduce dependency on specific EH interface ([`a7f4ab8`](https://github.com/winksaville/rp-hal/commit/a7f4ab83877b09d7b59799b7b5b2b895a0084578))
    - Fix Spi for EH1 alpha ([`967340b`](https://github.com/winksaville/rp-hal/commit/967340b63e261fa461edea60088d2c4a0c8a0952))
    - Update rp2040-e5 feature's doc to match latest fixes. ([`afec400`](https://github.com/winksaville/rp-hal/commit/afec400eb9aaa232d1e3c228129d612010930e2f))
    - Add missing SYSINFO in safety note. ([`a74cfdf`](https://github.com/winksaville/rp-hal/commit/a74cfdf210d1e354cdf2a54e2db665146a85122f))
    - Fix broken link to team list ([`9e3ec8d`](https://github.com/winksaville/rp-hal/commit/9e3ec8ddeb9ec1564ce95b72e735a9727ccfce63))
    - Abort early if bank0 is in reset with rp2040-e5 workaround active. ([`50f087c`](https://github.com/winksaville/rp-hal/commit/50f087cb57fb23d382cbf511bee6b52f9a19c18c))
    - Update comments & doc. ([`3e14a73`](https://github.com/winksaville/rp-hal/commit/3e14a73fb4fca6a19c9ff18cb3d6d803403b487a))
    - Add a check to bypass the workaround on rev B2 and above. ([`5f06461`](https://github.com/winksaville/rp-hal/commit/5f06461c6fe949c9fbafe01652d0a4dad3e7469b))
    - Improve usb errata 5 feature's documentation. ([`2810474`](https://github.com/winksaville/rp-hal/commit/281047401b0e72696809fc2be01d17bf122c527f))
    - Merge pull request #603 from Gip-Gip/byteswapping-config ([`6e9762a`](https://github.com/winksaville/rp-hal/commit/6e9762a92a6285ca2f9f2e6acd4e0f918776e0ad))
    - Actually build on-target-tests in CI ([`6391813`](https://github.com/winksaville/rp-hal/commit/6391813668cb7cf43a0a4291c4d3a08b1f1f6197))
    - Merge pull request #601 from jannic/issue-599 ([`b8d9124`](https://github.com/winksaville/rp-hal/commit/b8d91247e861ddad2fa7caf0cb8fbb41a1a5a015))
    - Document on-target tests ([`8ac9115`](https://github.com/winksaville/rp-hal/commit/8ac9115db4d51ed1a5fda9ed6d5c1a6396f8280e))
    - Remove on-target-tests/tests/dma_drop.rs ([`24ea504`](https://github.com/winksaville/rp-hal/commit/24ea504e62d5da9da37747b76a95523310643524))
    - Merge pull request #600 from jannic/dma_word_size_check ([`06b98e0`](https://github.com/winksaville/rp-hal/commit/06b98e060b752bd028591b68d89865dee92f95e5))
    - Remove dma_m2m_u64 on-target-test ([`d6b2c5e`](https://github.com/winksaville/rp-hal/commit/d6b2c5e0ac2faed8af5694041c0b54e85a536eef))
    - Ensure supported DMA word size at compile time ([`1291411`](https://github.com/winksaville/rp-hal/commit/129141103f3d30c75f0b7ac969e5878aeb2eb89f))
    - Merge pull request #597 from jannic/add-repo-link ([`cd4cb7b`](https://github.com/winksaville/rp-hal/commit/cd4cb7baea9db9fa116fa81a3737277f56e5a987))
    - Add repository link to Cargo.toml ([`f32826a`](https://github.com/winksaville/rp-hal/commit/f32826a0e69ffc07a6bf44b0b879f939dd27dc01))
    - Update changelog ([`a3a18bb`](https://github.com/winksaville/rp-hal/commit/a3a18bb6c5550228f7c33ff438b75465fd0b1770))
    - Update documentation ([`f0e6f71`](https://github.com/winksaville/rp-hal/commit/f0e6f71ee1f183952a33bd49d03f76735f582edc))
    - Remove the requirement for multicore tasks to never return ([`b6bfd6c`](https://github.com/winksaville/rp-hal/commit/b6bfd6c094f78baf1cfce429d02114dca0af3728))
    - Merge pull request #596 from jannic/prepare-release-0.8.1 ([`6ae5079`](https://github.com/winksaville/rp-hal/commit/6ae507911d5735d3cc176a8461d91cb17bd9bb6e))
    - Prepare release of version 0.8.1 ([`67e155e`](https://github.com/winksaville/rp-hal/commit/67e155ebac53e39b1626c20793beed2de9b66506))
    - Merge pull request #595 from ithinuel/update-changelog ([`b90daf5`](https://github.com/winksaville/rp-hal/commit/b90daf525a9df28aa2e113caf6420e88b37d1a10))
    - Update changelog in preparation of 0.8.1 ([`2c34d42`](https://github.com/winksaville/rp-hal/commit/2c34d4298dda2bd58f241ec2a0b925cde93e10ba))
    - Merge pull request #588 from ithinuel/improve-testing ([`c6c563f`](https://github.com/winksaville/rp-hal/commit/c6c563fc1ca261f404e2e9e4fda924f55023a95b))
    - Fix GH workflow's description for workspace's build step ([`ec8abe7`](https://github.com/winksaville/rp-hal/commit/ec8abe759c1c7e9d53cb50ae6480b616c21742e3))
    - Update rp2040-hal/src/dma/single_buffer.rs ([`5ae4852`](https://github.com/winksaville/rp-hal/commit/5ae485298b64ec9f4817e31e887c51e75a7fb891))
    - Update rp2040-hal/src/dma/bidirectional.rs ([`839896f`](https://github.com/winksaville/rp-hal/commit/839896f7f70e222130690d2d96eae7c77eb9afcb))
    - Update rp2040-hal/src/dma/double_buffer.rs ([`8dd3649`](https://github.com/winksaville/rp-hal/commit/8dd3649688ea1f1d0855cd41000f828494f51774))
    - Added config options for byteswapping ([`f2aa0cc`](https://github.com/winksaville/rp-hal/commit/f2aa0cc7307370a9da4888ce71967e90bf301db7))
    - Merge pull request #582 from jannic/update-eh-alpha ([`7e8ad86`](https://github.com/winksaville/rp-hal/commit/7e8ad868c2944de0f10f37b26e153ef9e9e960b8))
    - Bump on-target-tests rp2040-hal's version ([`208ed01`](https://github.com/winksaville/rp-hal/commit/208ed01d57af5923881f7e00ebb1db085d434542))
    - Use cargo hack to run feature combinasion ([`53eab80`](https://github.com/winksaville/rp-hal/commit/53eab80d9302dc11daced34880603d56aaced549))
    - Re-add iterator-based i2c methods ([`4f01102`](https://github.com/winksaville/rp-hal/commit/4f011020c33a0ca0ced4346029653a1ac4eb9fae))
    - Merge pull request #579 from jlpettersson/add_basic_dma_example ([`b24ada1`](https://github.com/winksaville/rp-hal/commit/b24ada1d935b3b6ec7a11cf9579902df72ee41dc))
    - Merge pull request #587 from jannic/clippy-check-exported-api ([`2c9921c`](https://github.com/winksaville/rp-hal/commit/2c9921cdc578bfcbd5c6e0eb0085bb91f9a7e229))
    - Dma example: Fix build issue and rename to mem_to_mem_dma ([`db04830`](https://github.com/winksaville/rp-hal/commit/db04830e0ce1b130299e0863a06ef24219e34632))
    - Update rp2040-hal/examples/dma.rs ([`ac7cb95`](https://github.com/winksaville/rp-hal/commit/ac7cb956b516c666dd0e15637055af8333397dd8))
    - Activate clippy checks on exported APIs ([`f5dc834`](https://github.com/winksaville/rp-hal/commit/f5dc834374a30f32a04f692ec404e024e022df88))
    - Merge pull request #586 from jannic/add-feature-docs ([`22121b5`](https://github.com/winksaville/rp-hal/commit/22121b5078ffe75d5f2c3b49cadc067dd5d9ecda))
    - Add documentation for crate features to lib.rs ([`fe380f1`](https://github.com/winksaville/rp-hal/commit/fe380f14b9f45f8e14ee8819db98b0483718f28f))
    - Merge pull request #583 from ArchUsr64/main ([`0d36ef9`](https://github.com/winksaville/rp-hal/commit/0d36ef992c518e04457aa10ae9fd0b829751409b))
    - Apply suggestions from code review ([`729ef82`](https://github.com/winksaville/rp-hal/commit/729ef8212fc26e96e095057b4a003846901d6bce))
    - Removed redundant type cast to u32 ([`3081dbb`](https://github.com/winksaville/rp-hal/commit/3081dbbb1a813a83502cae09bfcfe4066d3acb56))
    - Updated rp2040-hal dependency to testing fork ([`42e5e9b`](https://github.com/winksaville/rp-hal/commit/42e5e9b538b4f135322c874597114959585958e5))
    - Changed baudrate_dividers from u16 to u32 ([`c4420c8`](https://github.com/winksaville/rp-hal/commit/c4420c807352dee3b2c2aeca1bc9522ce3f1cf13))
    - Merge pull request #570 from jannic/timer-docs ([`8f6cbd8`](https://github.com/winksaville/rp-hal/commit/8f6cbd85c255bcd902e32bf41f33be85cd532ca1))
    - Fix a clippy warning ([`b10b828`](https://github.com/winksaville/rp-hal/commit/b10b8281e5847ba2d5e536d72d26bf6be6becfe9))
    - Remove functions which where removed from eh-alpha traits ([`ff4069a`](https://github.com/winksaville/rp-hal/commit/ff4069a338c5faee890690dcfefdc4a66c814533))
    - Impl eh1::Error for dynpin::Error ([`1e05bab`](https://github.com/winksaville/rp-hal/commit/1e05bab43b1ab66ce22051e7cefd975a0abfa6be))
    - Update embedded-hal alpha dependencies ([`b582de8`](https://github.com/winksaville/rp-hal/commit/b582de8815fd2fe30d6de04a8563dfee6f2bc209))
    - Merge pull request #580 from jlpettersson/fix_dma_irq_fn ([`9b7acef`](https://github.com/winksaville/rp-hal/commit/9b7acef8c0145cc595ef5861756fe5be5d99c8b2))
    - Fix DMA IRQ issue for bidirectional DMA transfer ([`3b20353`](https://github.com/winksaville/rp-hal/commit/3b20353b648ee4643884653309aed5a0e53f0645))
    - Add basic DMA example, memory to memory transfer ([`6332e8d`](https://github.com/winksaville/rp-hal/commit/6332e8def357663933f1683b4ac12eae1b0d950d))
    - Merge pull request #578 from jannic/define-ram-regions ([`29d57af`](https://github.com/winksaville/rp-hal/commit/29d57af9c61f83a67ac6787294f0b7132ec9d9cb))
    - Document RAM banks in memory.x ([`c7af7be`](https://github.com/winksaville/rp-hal/commit/c7af7bebac0cc9d0f26dad1fe3c8f9dd69d22161))
    - Merge pull request #577 from jlpettersson/fix_broken_link_in_rust-doc ([`b17df1d`](https://github.com/winksaville/rp-hal/commit/b17df1d1914a84c568ef501e8da993130470b0d6))
    - Fix a broken link in docs ([`7ff4748`](https://github.com/winksaville/rp-hal/commit/7ff4748f0940aef43be1e1213e23a8bf36576f2e))
    - Merge pull request #575 from jlpettersson/fix_probe-run_command ([`ac998ca`](https://github.com/winksaville/rp-hal/commit/ac998caf00c60a42eddadcff6f4bbcaba5d19fae))
    - Fix probe-run command in readme ([`61017f0`](https://github.com/winksaville/rp-hal/commit/61017f0341c7f4616925a76e50350131b2a0ec5d))
    - Merge pull request #574 from AkiyukiOkayasu/fix-typo ([`076a190`](https://github.com/winksaville/rp-hal/commit/076a190ab49f5a5f6a416018f6bf156c1adf6527))
    - Fix typo ([`b67e44c`](https://github.com/winksaville/rp-hal/commit/b67e44c3752801d15652d11d4d9d96a8c12fee37))
    - Remove unused syn feature extra-traits ([`f12fb71`](https://github.com/winksaville/rp-hal/commit/f12fb71711b342ed06a04b4dc2ede52a089495c7))
    - Upgrade syn to version 2.0 ([`faafef7`](https://github.com/winksaville/rp-hal/commit/faafef77d69f470566a1b582def693dd9e27f6ef))
    - Fix code in doc comment ([`c6ced31`](https://github.com/winksaville/rp-hal/commit/c6ced31ada7c26934c8289b47178d612ee52dc23))
    - Mention clock initialization in timer docs ([`f29abee`](https://github.com/winksaville/rp-hal/commit/f29abee0d067dec35eae89129c3c9c9cce1ec35e))
    - Merge pull request #558 from jannic/adc ([`715c3c9`](https://github.com/winksaville/rp-hal/commit/715c3c9dd85f4b30d949c310b60e7621ea62c3f6))
    - Merge pull request #569 from jannic/eh-alpha-nb ([`b75e94e`](https://github.com/winksaville/rp-hal/commit/b75e94e00b4205d6c8a2f8cf8190befbfd3d9803))
    - Add implementations for alpha embedded-hal-nb traits ([`2a1ba85`](https://github.com/winksaville/rp-hal/commit/2a1ba85490b05fcfda06e329d33fac3d6b36daea))
    - Merge pull request #566 from Gip-Gip/main ([`6e46827`](https://github.com/winksaville/rp-hal/commit/6e4682791945ec7482bf1f20fabf72055662d7f1))
    - Update documentation to rp2040-hal/src/pio.rs ([`91442fc`](https://github.com/winksaville/rp-hal/commit/91442fc28da6d309b8f2de48054c353af9bd9445))
    - Merge pull request #567 from jannic/doc ([`c4f774c`](https://github.com/winksaville/rp-hal/commit/c4f774c17c51eed4d8df7d7f3d682ee068a00885))
    - Minor formatting improvement in doc comment ([`5bccf47`](https://github.com/winksaville/rp-hal/commit/5bccf4739036cc40ee80c74792fe9cf3fd13c29c))
    - Added set_mov_status_config function to PIOBuilder ([`9456165`](https://github.com/winksaville/rp-hal/commit/94561658f470d558c500bb7203882ad90ca171ee))
    - Merge pull request #562 from jannic/pwm_has_overflown ([`9b857e3`](https://github.com/winksaville/rp-hal/commit/9b857e34366531bd066443d7420f9436c8381a22))
    - Update comment in rp2040-hal/src/pwm/mod.rs ([`f9beeeb`](https://github.com/winksaville/rp-hal/commit/f9beeeb299a0f814b4ec89495eb4d94d227e0506))
    - Add CHANGELOG entry ([`beb2eda`](https://github.com/winksaville/rp-hal/commit/beb2eda202e6138eeb2e15c80499764a2901523c))
    - Read `intr` instead of `ints` in `pwm::Slice::has_overflown` ([`89535e1`](https://github.com/winksaville/rp-hal/commit/89535e18b81962eaa055bedb2705b3869fe65812))
    - Use name TEMPERATURE_SENSOR_CHANNEL instead of numeric value ([`b1e63b8`](https://github.com/winksaville/rp-hal/commit/b1e63b86057c94180e6953119d4b3731423329c5))
    - Merge pull request #555 from jannic/update-actions ([`aaa306f`](https://github.com/winksaville/rp-hal/commit/aaa306fddf01b706ab4b88d7b7edcb1d8d9263e9))
    - Update github actions ([`8b20770`](https://github.com/winksaville/rp-hal/commit/8b207705479110ef7e3e6ab848f58ac129196069))
    - Merge pull request #551 from rp-rs/prepare-release-0.8.0 ([`f6a0d1b`](https://github.com/winksaville/rp-hal/commit/f6a0d1b944b4fea3b09e8826dd9a8d8145c52442))
    - Update rp2040-hal/CHANGELOG.md ([`1218fb5`](https://github.com/winksaville/rp-hal/commit/1218fb5efd06234b6876ece8b6a370fa866ce5ea))
    - Prepare release of version 0.8.0 ([`94313d5`](https://github.com/winksaville/rp-hal/commit/94313d5f34421b44f60127f6123d49733d1babb5))
    - Mention changes from #541 in changelog ([`d2f2ad4`](https://github.com/winksaville/rp-hal/commit/d2f2ad412d27cc322dab6cb95e8d57ce2f73445c))
    - Merge pull request #541 from dlkj/remove-pwm-pin-token ([`e588b4a`](https://github.com/winksaville/rp-hal/commit/e588b4a7b48e19f101537252056b463bde4e0522))
    - Merge pull request #549 from jannic/sealed-traits ([`636992e`](https://github.com/winksaville/rp-hal/commit/636992e311bdd0a457e5797208a1c0b888756208))
    - Avoid repetitions of spinlock macro ([`e59b45f`](https://github.com/winksaville/rp-hal/commit/e59b45fab4f66db6348a6aa212e8a7049bff0d06))
    - Update CHANGELOG ([`0ee88e6`](https://github.com/winksaville/rp-hal/commit/0ee88e6da10b262d564baea301a2b0f4629237e8))
    - Seal several traits ([`2c81897`](https://github.com/winksaville/rp-hal/commit/2c818978c6850d7335aee977a6e8ba9def46c8eb))
    - Merge pull request #548 from jannic/changelog ([`1e57c16`](https://github.com/winksaville/rp-hal/commit/1e57c16957eafe41ae81e013643c6bf2e9d08fb2))
    - Update README - DMA support was not only added for UART ([`c4b6c7b`](https://github.com/winksaville/rp-hal/commit/c4b6c7bcaf6e09f09792029374e1e012e83deb13))
    - Update CHANGELOG ([`82d9fdc`](https://github.com/winksaville/rp-hal/commit/82d9fdcf79d95c285b8ff8d55590f0ad8d60c87a))
    - Merge pull request #543 from tomgilligan/feature/InterpBase1And0 ([`d95009c`](https://github.com/winksaville/rp-hal/commit/d95009c43cf4e8963bbd5b3e889419e560a1b869))
    - Merge pull request #546 from jannic/rust-version ([`1bfdffd`](https://github.com/winksaville/rp-hal/commit/1bfdffda9a97fc80c3cd97bc0f2ec9479ecb7fbf))
    - Merge branch 'rp-rs:main' into remove-pwm-pin-token ([`9af6bad`](https://github.com/winksaville/rp-hal/commit/9af6badc0d63d396a3241fdb01af29aa2b1c2e97))
    - Set MSRV to 1.62 ([`637a939`](https://github.com/winksaville/rp-hal/commit/637a939a1f708515fa64a194e2d72c03ec7465e0))
    - Add check for MSRV ([`9b78d49`](https://github.com/winksaville/rp-hal/commit/9b78d49c3378248707a0c3953d099ef6d2792980))
    - Merge pull request #537 from zaksabeast/spi-slave ([`85ce865`](https://github.com/winksaville/rp-hal/commit/85ce865818601f7b8a43d445845d4f3ccb295145))
    - Merge pull request #545 from jannic/fix-new-clippy-warning ([`7e4b601`](https://github.com/winksaville/rp-hal/commit/7e4b601a4a453f0215fd6f6a364d1c293978258d))
    - Fix clippy warning 'uninlined-format-args' ([`c4ad61b`](https://github.com/winksaville/rp-hal/commit/c4ad61b7372a0889349094b76b69bf4904986608))
    - Use dummy values for frequency and baudrate ([`d033ee4`](https://github.com/winksaville/rp-hal/commit/d033ee45c0ebe12ff25be2e5a5a3ef6c1a23ba52))
    - Split spi init into slave and master ([`1a2d894`](https://github.com/winksaville/rp-hal/commit/1a2d8943b7f602bdb5cc35aac28c01567b2f4351))
    - Add set_base_1and0 used by simple_blend3 interp example ([`55a4e14`](https://github.com/winksaville/rp-hal/commit/55a4e1485e597d557122d2011c6c6807b10e0f83))
    - Fix typo ([`ed10f0c`](https://github.com/winksaville/rp-hal/commit/ed10f0c908e17bc462340648fc8fa689b7c4dfca))
    - Fix typo ([`79c67df`](https://github.com/winksaville/rp-hal/commit/79c67df31fe492ef5860c7619a525fd0f9a6b7f5))
    - Fix typo ([`be30a48`](https://github.com/winksaville/rp-hal/commit/be30a48e95babbb6ed1414e5baf3fdec48fa0bd8))
    - Remove pwm::PwmPinToken ([`e60f640`](https://github.com/winksaville/rp-hal/commit/e60f6405744eeff7db28ee22a20ce1aa0dafc57d))
    - Add pwm irq input example ([`19c03e0`](https://github.com/winksaville/rp-hal/commit/19c03e0106699d7ec13afcb4d2dda3f932a836bd))
    - Merge pull request #540 from nmattia/nm-finished-comment ([`e785a69`](https://github.com/winksaville/rp-hal/commit/e785a690440d7d5a5f24e7b4645b192703d17e00))
    - Merge pull request #539 from nmattia/nm-io-comment-swap ([`66c52d3`](https://github.com/winksaville/rp-hal/commit/66c52d3c782e97c79c87924f95c0bfe89a7cef7f))
    - Clarify 'finished()' behavior for alarms ([`e7153c8`](https://github.com/winksaville/rp-hal/commit/e7153c8418484fc438fd9cead183c049ed736b9c))
    - Fix ValidPwmPin trait comments ([`d4ba722`](https://github.com/winksaville/rp-hal/commit/d4ba7222c21817e17d0a76cbf8c2c508cdeaa5b9))
    - Add spi slave ([`afd42d6`](https://github.com/winksaville/rp-hal/commit/afd42d6b59d033ef87f98603d992ba6ee7b4ab4f))
    - Merge pull request #489 from ithinuel/check-rp2040-hal-without-bsps ([`ec6f34a`](https://github.com/winksaville/rp-hal/commit/ec6f34a842a718c4d7029e499b23f3e3ba6a4b34))
    - Merge pull request #529 from tianrking/patch-1 ([`05fe322`](https://github.com/winksaville/rp-hal/commit/05fe322c46d48fef8538a7aa4992a719dcee45a1))
    - Merge pull request #532 from jannic/update-actions ([`c915135`](https://github.com/winksaville/rp-hal/commit/c9151357f0d5ba988bbe04ebbc9284b4c21fdd87))
    - Specify toolchain using @rev of rust-toolchain action ([`4bf1318`](https://github.com/winksaville/rp-hal/commit/4bf1318f706ae5cc4b75a3240b710666e066eff6))
    - Replace actions-rs/cargo@v1 with direct cargo calls ([`b00aa0c`](https://github.com/winksaville/rp-hal/commit/b00aa0c19ff8758b3339c0bfb2085bb7b3f44fb9))
    - Use github action dtolnay/rust-toolchain@master instead of actions-rs/toolchain@v1 ([`1a7e88e`](https://github.com/winksaville/rp-hal/commit/1a7e88e3e422455b1c2f9571343e2686ca6dd5cf))
    - Update github workflows to actions/checkout@v3 ([`d9e8f5f`](https://github.com/winksaville/rp-hal/commit/d9e8f5ff3aafa86aa9d0d42e57a81fa9ca3f9f2a))
    - Merge pull request #523 from MuratUrsavas/add-alarm-cancellation ([`1333dd7`](https://github.com/winksaville/rp-hal/commit/1333dd763b05843302d8741dd054de3c06c05d68))
    - Merge pull request #524 from jannic/add-pin-id ([`bf126d5`](https://github.com/winksaville/rp-hal/commit/bf126d5f09e0d1a686a89e88a89abaf0a2e191e7))
    - Example application name ([`5a2ae8e`](https://github.com/winksaville/rp-hal/commit/5a2ae8e7a2ffd01e0325dbfa7033b9d12237688b))
    - Merge pull request #526 from jannic/improve-comment ([`25649ba`](https://github.com/winksaville/rp-hal/commit/25649ba520defed03585b25a440702d504cdbeb9))
    - Disambiguate a comment ([`94e70ac`](https://github.com/winksaville/rp-hal/commit/94e70aca9062206d3ec7596083ebbfa48aa879e8))
    - Fix doctests ([`769ec0b`](https://github.com/winksaville/rp-hal/commit/769ec0b03dccd0addcbb68d697bdc7ed409b9cc4))
    - Added Alarm cancellation feature. ([`0e66889`](https://github.com/winksaville/rp-hal/commit/0e668899099e541632d23ad73b5d193722d32e8f))
    - Add Pin::id() ([`b54f4a4`](https://github.com/winksaville/rp-hal/commit/b54f4a44f70e1196280bfbefc7e854ec643373e7))
    - Merge pull request #519 from larsarv/dynpin_interrupts ([`aaa66b9`](https://github.com/winksaville/rp-hal/commit/aaa66b929ef846b05bd8b6ad87b068bd35751639))
    - Fix formating to pass cargo fmt check ([`583b6de`](https://github.com/winksaville/rp-hal/commit/583b6deeee26920df7370cc95234cea3d21bf462))
    - Merge pull request #521 from jannic/fix-changelog ([`cf3a216`](https://github.com/winksaville/rp-hal/commit/cf3a2169c2ef72eba0f40e92a56fc45a33c421dc))
    - Add a missing changelog entry for the 0.7.0 release ([`74a5541`](https://github.com/winksaville/rp-hal/commit/74a55412c2803593537f6426c9ac89caadb87620))
    - Fix use ([`f79a072`](https://github.com/winksaville/rp-hal/commit/f79a0729d6a417476fe71c73e6153fb3de32a9ea))
    - Interrupt functions for DynPin ([`be98026`](https://github.com/winksaville/rp-hal/commit/be98026da6a4526150c44dd92f6592b9456158c1))
    - Merge pull request #518 from jannic/prepare-release-0.7.0 ([`4c8e16a`](https://github.com/winksaville/rp-hal/commit/4c8e16aec9373fdeac0e5af2d4ec06fbc999b302))
    - Fix links to demos ([`88ca22a`](https://github.com/winksaville/rp-hal/commit/88ca22a7b1524a07c9bcc0c62d8004d2ec782ab6))
    - Prepare for HAL 0.7.0 release ([`69781df`](https://github.com/winksaville/rp-hal/commit/69781df551174c68c30a1da3368006c2726d1191))
    - Merge pull request #517 from jannic/move-boards ([`18ee0ed`](https://github.com/winksaville/rp-hal/commit/18ee0edfcd089eed58abc5283bb426684eac44be))
    - Remove unused dependency on cortex-m-rt ([`69f34e8`](https://github.com/winksaville/rp-hal/commit/69f34e87a895b58dedd1f1865b08d26dba064f47))
    - Updated READMEs, CHANGELOG ([`a14604a`](https://github.com/winksaville/rp-hal/commit/a14604a2225f0f36d542aea2c9adabfd5334c180))
    - Remove BSP crates ([`6e8d75d`](https://github.com/winksaville/rp-hal/commit/6e8d75d42c098b6e158e361ae71f9debf9d8e6bc))
    - Merge pull request #514 from jannic/update-changelog ([`06a6e18`](https://github.com/winksaville/rp-hal/commit/06a6e18862d05456cc541b8dd75ee2005a580a82))
    - Update CHANGELOG.md ([`b80833a`](https://github.com/winksaville/rp-hal/commit/b80833ad62bb9842a05d918f242b07bdd31e21d0))
    - Merge pull request #506 from jannic/issue-503 ([`2a5b0ce`](https://github.com/winksaville/rp-hal/commit/2a5b0ce01eba438b2e4f915211bcf1d90f85c4ce))
    - Use generic boot loader for arduino nano connect ([`1c6a816`](https://github.com/winksaville/rp-hal/commit/1c6a816182632b01f9a9236709e44eb8272cd31d))
    - Merge pull request #502 from jannic/remove-critical-section-0.2 ([`6fca82f`](https://github.com/winksaville/rp-hal/commit/6fca82f810fbf24e806f397279bcfe5d13ce57a4))
    - Remove support for deprecated version 0.2 of critical-section ([`e3a6612`](https://github.com/winksaville/rp-hal/commit/e3a6612366d36cb4ca00b59c89d6e3c7ff9a905e))
    - Merge pull request #494 from jannic/pio-change-clkdiv ([`4b2b33b`](https://github.com/winksaville/rp-hal/commit/4b2b33b950d06ad690cde7088db2545e39f02221))
    - Merge pull request #497 from jannic/dead-code-RpSpinlockCs ([`f00ea66`](https://github.com/winksaville/rp-hal/commit/f00ea66ccd64256e28ee7257a949614841a89017))
    - Merge pull request #496 from icedrocket/main ([`40f3f42`](https://github.com/winksaville/rp-hal/commit/40f3f42c705f5778f53c7db203f6546e881f307c))
    - Avoid dead_code warning if critical-section-impl is not enabled ([`c198843`](https://github.com/winksaville/rp-hal/commit/c1988432c8054fb6d46fb105cc19b78f5fc777dc))
    - Add docs.rs metadata ([`1b72a48`](https://github.com/winksaville/rp-hal/commit/1b72a48870a49ecb66dff91b6053086ee94d11ec))
    - Merge pull request #495 from jannic/minor-readme-update ([`3744a75`](https://github.com/winksaville/rp-hal/commit/3744a75ba3e43836b843ffa8e59254d3b7cdabc8))
    - Update rp2040-hal version in README.md ([`caea9ec`](https://github.com/winksaville/rp-hal/commit/caea9ecfd7976f444165d76d5e41b2b11e339ce8))
    - Update doc comment of set_clock_divisor, clock_divisor_fixed_point ([`2f077a4`](https://github.com/winksaville/rp-hal/commit/2f077a434baa448c3b84cba32e8d51f7e384497f))
    - Allow setting clock divisors on running state machines ([`81da6f1`](https://github.com/winksaville/rp-hal/commit/81da6f12fef54e9f6e0a8c97f38b59ab4b2b6b16))
    - Merge pull request #484 from davidcole1340/program-wrap ([`0ecf274`](https://github.com/winksaville/rp-hal/commit/0ecf27450ab0e53e7d7ceea5ce8f84340c97ec81))
    - Merge pull request #473 from jannic/update-changelog ([`f0d7cd9`](https://github.com/winksaville/rp-hal/commit/f0d7cd998fcd5d888828d082678a64246251e6bb))
    - Merge pull request #490 from jannic/pico_usb_serial_fmt_string ([`e921ce0`](https://github.com/winksaville/rp-hal/commit/e921ce06b4b477de2e755104d0913df187fc2f09))
    - Extend pico_usb_serial example with some string formatting ([`4c6600e`](https://github.com/winksaville/rp-hal/commit/4c6600e03694fb7df209235b2fe211acbfaa8017))
    - Merge pull request #488 from ptpaterson/eh1_0_alpha-spi ([`5ae1f90`](https://github.com/winksaville/rp-hal/commit/5ae1f909399317ec555cd350b014296088d01186))
    - Merge pull request #486 from 9names/error_add_debug_traits ([`9bc48de`](https://github.com/winksaville/rp-hal/commit/9bc48de974ed03ee68b25d31535899fa6689b17c))
    - Amend CI to build rp2040-hal without the bsp's features. ([`77ecdde`](https://github.com/winksaville/rp-hal/commit/77ecdde48ea28b90bb085a8bd84c525e8892ed9e))
    - Implement embedded-hal aplha SPI traits ([`98daa7a`](https://github.com/winksaville/rp-hal/commit/98daa7a25df2e20faa8c676b1d2a97460d2713a6))
    - Merge pull request #483 from zachs18/patch-1 ([`e60a979`](https://github.com/winksaville/rp-hal/commit/e60a979edad548c4091425ba0718d8146b27676c))
    - Update rp2040-hal/CHANGELOG.md ([`4ca2dcf`](https://github.com/winksaville/rp-hal/commit/4ca2dcfd20cd9e3709feef0190366b9f3e78a5bb))
    - Add derive(Debug) and derive(defmt::Format) to error types ([`219d393`](https://github.com/winksaville/rp-hal/commit/219d3930850cdbdd01c013343e2a290f72c01ab9))
    - Do not include offset when checking wrap bounds ([`3c06a33`](https://github.com/winksaville/rp-hal/commit/3c06a3359e2c9ab6208ed180cb1eaa01c21f1f94))
    - Add ability to modify installed program wrap bounds ([`1ba07b0`](https://github.com/winksaville/rp-hal/commit/1ba07b09e780a2c01ec3e3c052eaa28bcd250d2a))
    - Merge pull request #467 from jannic/fix-466 ([`8e79f43`](https://github.com/winksaville/rp-hal/commit/8e79f438ba2f33226f9f9b5e6adc7430b141411a))
    - Remove unnecessary `mut` from `static mut LOCK_OWNER: AtomicU8` in critical section impl. ([`2b8dda7`](https://github.com/winksaville/rp-hal/commit/2b8dda74aa22b7dc7307bcdfda09b0efe356aa9f))
    - Merge pull request #479 from tweksteen/bump_version_doc ([`3a0b33c`](https://github.com/winksaville/rp-hal/commit/3a0b33cfc8087c3d49befe97351f0ed51baf5b2f))
    - Bump rp-pico version in README.md ([`578657a`](https://github.com/winksaville/rp-hal/commit/578657a82978b47d11dee41399124ff12ad8bd34))
    - Merge pull request #474 from jannic/update-pac ([`2fb3e2a`](https://github.com/winksaville/rp-hal/commit/2fb3e2a7e96cc9901d38c24b4a60b9960d90e866))
    - Update dependency on rp2040-pac to 0.4.0 ([`018965d`](https://github.com/winksaville/rp-hal/commit/018965d015156ff9931478f06370801295cce8b2))
    - Update CHANGELOG ([`95598ad`](https://github.com/winksaville/rp-hal/commit/95598ad19946141b603c26a25d9bf7a14ca12eee))
    - Merge pull request #472 from Sizurka/uart-rx-discard ([`2b941db`](https://github.com/winksaville/rp-hal/commit/2b941db745fc86f84dfecb837cc4417aaad32e65))
    - Add CHANGELOG entry for UART error field ([`04e2458`](https://github.com/winksaville/rp-hal/commit/04e245813a55cc360df6849eb1bfb064a8598a14))
    - Fix UART read error discard data ([`c461d21`](https://github.com/winksaville/rp-hal/commit/c461d21136df52d615955d59387869173b57ae97))
    - Merge pull request #471 from jannic/uart-config-constructor ([`de673fb`](https://github.com/winksaville/rp-hal/commit/de673fb192949370c4668f569a0d2adedcfbec72))
    - Make UartConfig::new(...) const ([`d8a0c64`](https://github.com/winksaville/rp-hal/commit/d8a0c6461842bcee3389c3e8e98a3a1a038d2868))
    - Add CHANGELOG entries ([`e9428c3`](https://github.com/winksaville/rp-hal/commit/e9428c3f57a14f9aa6d0bf3097bb308e42e86205))
    - Add deprecation attribute to common_configs ([`fb7fba0`](https://github.com/winksaville/rp-hal/commit/fb7fba03ad86e94aa74a5cf8e55665ef0a983c07))
    - Use UartConfig::new constructor instead of common_configs in examples ([`b81ad6f`](https://github.com/winksaville/rp-hal/commit/b81ad6f599b9b0985e74117ad9388f3d35182bd7))
    - Implement UartConfig::new constructor method ([`0a86dad`](https://github.com/winksaville/rp-hal/commit/0a86dad34ccc99c339138997035bae90257ad2c1))
    - Merge pull request #468 from jannic/fix-465 ([`71c39a4`](https://github.com/winksaville/rp-hal/commit/71c39a44317638fa9cb80abcd8c51219a180b7e5))
    - Check watchdog load value max value before multiplying by 2, to avoid integer overflow ([`84b92ed`](https://github.com/winksaville/rp-hal/commit/84b92edd3012206785dcfae38050468f2aec3706))
    - Use InstalledProgram::share() in examples/pio_synchronized.rs ([`e9923cb`](https://github.com/winksaville/rp-hal/commit/e9923cbcd2da55c69e1ea563085bb1ad8e37d5aa))
    - Merge pull request #462 from 9names/bsp_enable_cache ([`82800fe`](https://github.com/winksaville/rp-hal/commit/82800fe370c521d404fbd1bfa10621605b6fd056))
    - Add rom-func-cache as a default feature in BSPs ([`2d31d91`](https://github.com/winksaville/rp-hal/commit/2d31d91ba1339097419e25b4c1f9cebb5c89de59))
    - Comment and pass-through HAL features in BSPs ([`0cd990c`](https://github.com/winksaville/rp-hal/commit/0cd990c3c18bb17f4f89f7a64938fcc717bfd2d2))
    - Add comments for HAL features ([`fc110f0`](https://github.com/winksaville/rp-hal/commit/fc110f07c3c533d9ec6cd061c4b018f70381852e))
    - Merge pull request #461 from jannic/upgrade-eh-alpha ([`6a040a8`](https://github.com/winksaville/rp-hal/commit/6a040a804216e797d67ad0bb2b679ad6e7911551))
    - Fix typo in changelog ([`d5bfb0c`](https://github.com/winksaville/rp-hal/commit/d5bfb0ca8da4a7cfe4f6f2af27099fb1eb7b84c5))
    - Update changelog ([`819f051`](https://github.com/winksaville/rp-hal/commit/819f051cc2812c349b8890e0d306793bd9feee39))
    - Remove unnecessary custom Infallible types ([`fcd6f7c`](https://github.com/winksaville/rp-hal/commit/fcd6f7c19d566d8e80204b3715eb5a15a1fb4bc3))
    - Upgraded embedded-hal alpha dependency to 1.0.0-alpha.9 ([`e4deaab`](https://github.com/winksaville/rp-hal/commit/e4deaabb518c65fc638240e3c131c34dc429f118))
    - Merge pull request #453 from jannic/update-jmp-offset ([`8d9b453`](https://github.com/winksaville/rp-hal/commit/8d9b4538c9d00969926fb0d3cee0b0e91db7de78))
    - Update Servo 2040 board examples in README ([`4f440d2`](https://github.com/winksaville/rp-hal/commit/4f440d286d81221e9ff4ee3d61aac7b2daebc4a5))
    - Fix servo example in rp2040-servo, remove unusable aliases. ([`d3b0156`](https://github.com/winksaville/rp-hal/commit/d3b01562690a3127f068f96e667f905765d0b9ad))
    - Merge pull request #455 from papyDoctor/spi-isbusy ([`e745408`](https://github.com/winksaville/rp-hal/commit/e7454087d181cafed9dbb10a34b54c709c9636dc))
    - Added SPI is_busy function ([`69c0471`](https://github.com/winksaville/rp-hal/commit/69c047136cbe05958bd4538e66f5243e52e7e38a))
    - Use u8 instead of usize for pio address calculation ([`6a5747b`](https://github.com/winksaville/rp-hal/commit/6a5747b213f5803216f85e6604d605f9bf4950e9))
    - Simplify jump offset calculation when loading PIO programs ([`7cca9a7`](https://github.com/winksaville/rp-hal/commit/7cca9a71d712b50f40e89fd1a47fa18b9354b3b9))
    - Merge pull request #452 from jannic/into_mode_setting_output ([`ae629ad`](https://github.com/winksaville/rp-hal/commit/ae629ad4c9d7dd05a5ee588f0bd940d0f974df5f))
    - Provide rp2040_hal::gpio::pin::Pin::into_push_pull_output_in_state ([`fa83510`](https://github.com/winksaville/rp-hal/commit/fa83510277ede8ab53f2b1cde9bca438473c079b))
    - Merge pull request #449 from papyDoctor/main ([`cbed259`](https://github.com/winksaville/rp-hal/commit/cbed25944a23015640176c59f96fdaaf401adaed))
    - Added set_fifos/set_rx_watermark/set_tx_watermark that permit to enable/disable the Rx/Tx FIFOs and to set the watermarks for the DMA/interrupts triggering ([`b29cc26`](https://github.com/winksaville/rp-hal/commit/b29cc2630c18387ee78535a61f4c96c3740dc82c))
    - Merge pull request #444 from jannic/critical-section-default ([`e681b67`](https://github.com/winksaville/rp-hal/commit/e681b67d9c10b30b1dbee7b26d523dcd25a65a7f))
    - Merge pull request #432 from jannic/fix-set_pindirs ([`00f5e8d`](https://github.com/winksaville/rp-hal/commit/00f5e8d1844c3839b2352b2c51ff7e4796631d76))
    - Temporarily disable out_sticky in set_pindirs ([`6b0ea14`](https://github.com/winksaville/rp-hal/commit/6b0ea14ec120e8c108745fea008555e24c10365f))
    - The patches to -pio need to be commented out before release. ([`cd9570e`](https://github.com/winksaville/rp-hal/commit/cd9570e7c439cc334ee3ae864ea86c7ce4ac497d))
    - Bump -pio dependencies ([`bf66ae9`](https://github.com/winksaville/rp-hal/commit/bf66ae9a58773e3c95de0bab919f359f118d81fd))
    - Bump pio version on boards still using pio 0.1.0 ([`e5eda48`](https://github.com/winksaville/rp-hal/commit/e5eda488916217ac50aaea9ac44ba65910b22f7a))
    - Migrate rp2040-hal from embedded_time to fugit ([`93ec18b`](https://github.com/winksaville/rp-hal/commit/93ec18be07f3a19f87ea6eefba4135b025c1533a))
    - Make the i2c error render as text if eh1_0_alpha is on. ([`6a29b3b`](https://github.com/winksaville/rp-hal/commit/6a29b3bb73748c131d104bed1169dc7bd284a576))
    - Enable critical-section-impl by default only from board crates, not from hal ([`280de7c`](https://github.com/winksaville/rp-hal/commit/280de7cb99be87f291b7b07c1c52cab8230a1a61))
    - Merge pull request #428 from jannic/fix-embedded-sdmmc-2 ([`6ef6838`](https://github.com/winksaville/rp-hal/commit/6ef6838132d35281522519f6e39f925c5f938a83))
    - Minimal fix for embedded-sdmmc build failure ([`d5331d1`](https://github.com/winksaville/rp-hal/commit/d5331d1ac7b50f7821c4658140b48ede815fe4ec))
    - Merge pull request #425 from camrbuss/clocks_extended_doc ([`735597b`](https://github.com/winksaville/rp-hal/commit/735597b14524b15776a731408aaf487e2d828e21))
    - Fix clocks extended usage xosc order ([`fea35b4`](https://github.com/winksaville/rp-hal/commit/fea35b48bbfae75812dc7ab0ee78a70ffbc42985))
    - Merge pull request #421 from jannic/issue-420 ([`f8bf06c`](https://github.com/winksaville/rp-hal/commit/f8bf06cb7f625959ea4e952a1576f4c736d9c987))
    - Enable rp2040-hal/defmt feature in dev-dependencies ([`68eb48b`](https://github.com/winksaville/rp-hal/commit/68eb48be44d2c775d2d20c838956619e8cb9c274))
    - Merge pull request #414 from jannic/critical-section-1.0.0 ([`ead6c26`](https://github.com/winksaville/rp-hal/commit/ead6c26eee2c599855945b9745962e7c9c05a002))
    - Feature-gate critical-section-impl ([`c1c5e05`](https://github.com/winksaville/rp-hal/commit/c1c5e05989f3fbf676d6f149e806d535d64a273d))
    - Update to critical-section 1.0.0 ([`b4d0d61`](https://github.com/winksaville/rp-hal/commit/b4d0d613e3d641f400a1c71278339621c2920cc9))
    - Merge pull request #418 from ithinuel/give-names-to-gha-steps ([`9792408`](https://github.com/winksaville/rp-hal/commit/9792408902ccde52eeab4e7611a84ee11ede122a))
    - Use matrix in GHA workflow to reduce duplication ([`082281b`](https://github.com/winksaville/rp-hal/commit/082281b10b96aa0a16f3b4a3a4a29f0c806b4539))
    - Merge pull request #419 from alxpettit/patch-1 ([`7e178ac`](https://github.com/winksaville/rp-hal/commit/7e178acde5a1bfdee1d7490fa703eaa750bf0779))
    - Update pico_usb_twitchy_mouse.rs ([`2635642`](https://github.com/winksaville/rp-hal/commit/26356428bf81cc15b9c5a52350c92d7a7600c27e))
    - Add meaningful names to steps and remove quasi-repetition ([`f10c73f`](https://github.com/winksaville/rp-hal/commit/f10c73f4fa92f3a35665cdb060063f0f3dcf2bd8))
    - Merge pull request #417 from jannic/clippy ([`fbba375`](https://github.com/winksaville/rp-hal/commit/fbba3755ff76c2f4cb8a00db6ce7c52781dd9894))
    - Fix clippy warnings ([`c1df2be`](https://github.com/winksaville/rp-hal/commit/c1df2bea2b1d2537edd70fc68cc30bf4f62d956f))
    - Merge pull request #415 from jannic/features-vector_table ([`96e15ee`](https://github.com/winksaville/rp-hal/commit/96e15ee6de2bd6902b74f62541292bd602b65701))
    - Merge pull request #416 from jannic/generic-boot-loader ([`e9a720f`](https://github.com/winksaville/rp-hal/commit/e9a720ffab6604f585cde7df3899fad23624e98f))
    - Enable feature "rt" when compiling vector_table example ([`0f33d2b`](https://github.com/winksaville/rp-hal/commit/0f33d2b8a632d313ee45fca05360979eff59bea6))
    - Use generic boot loader for rp2040-hal examples ([`d474306`](https://github.com/winksaville/rp-hal/commit/d4743061fa39ed87d6fe5403c39d511946d96cfa))
    - Merge pull request #408 from jannic/wfi ([`575aba4`](https://github.com/winksaville/rp-hal/commit/575aba4bfef5c530dca69cb2816e384d8131fb44))
    - Merge pull request #411 from jannic/fix-usb-sie_status ([`62f1ab2`](https://github.com/winksaville/rp-hal/commit/62f1ab2159a4beff46e42f25e32d56bb723340f4))
    - Clear sie_status.suspended / sie_status.resume flags in poll() ([`b636afb`](https://github.com/winksaville/rp-hal/commit/b636afb7b513cc9027a33659a58373106e4a3958))
    - To clear a bit in sie_status, just write that single bit ([`786062a`](https://github.com/winksaville/rp-hal/commit/786062aa74dc9d160d13e104b9d7991525ac8b1f))
    - Merge pull request #398 from jannic/defmt-0.3 ([`5448a12`](https://github.com/winksaville/rp-hal/commit/5448a12b31a54c0df72410d7dd4e2ff0bad288a3))
    - Merge pull request #410 from ithinuel/bump-usb-device-to-0-2-9 ([`fb9bac5`](https://github.com/winksaville/rp-hal/commit/fb9bac5064c2f84ce878b426e8bcf329b09fd65c))
    - Merge pull request #407 from FlorianUekermann/main ([`1be329a`](https://github.com/winksaville/rp-hal/commit/1be329a907f0df84765a11e41e1485f1ac826165))
    - Bump usb-device to 0.2.9 ([`60677df`](https://github.com/winksaville/rp-hal/commit/60677df09984187283d87c0b8cdff4a54410826f))
    - Use wfi in otherwise empty infinite loops in examples ([`4401978`](https://github.com/winksaville/rp-hal/commit/44019781e225101123898f824db3641d368db841))
    - Merge pull request #405 from ithinuel/fix-usb-ep0-out ([`6dafcc1`](https://github.com/winksaville/rp-hal/commit/6dafcc1ac0be328c1c9abc40250db679b945f262))
    - Implement NonPwmPinMode for gpio::Disabled ([`03e791a`](https://github.com/winksaville/rp-hal/commit/03e791ab31ba810c6491bbd582de4185cdde3fa0))
    - Remove defmt dependencies from boards/vcc-gnd-yd-rp2040/Cargo.toml ([`dfaeba5`](https://github.com/winksaville/rp-hal/commit/dfaeba5315670917dc551cdec98232ad0c482cd9))
    - Fix building of examples which do not use defmt ([`365ac70`](https://github.com/winksaville/rp-hal/commit/365ac70ae43792f42ac1f15c82ec3d09bba60bc2))
    - Merge pull request #406 from ithinuel/add-suspend-and-remote-wakeup-support ([`b1fcb7e`](https://github.com/winksaville/rp-hal/commit/b1fcb7eff8838715958d4a5f9767b57423908a02))
    - Add suspend, resume and remote wakeup support. ([`5dd095b`](https://github.com/winksaville/rp-hal/commit/5dd095bd45e68a08ad3af643f3305d8acdb401a0))
    - Fix missed ep0-data-out transaction ([`fa7c927`](https://github.com/winksaville/rp-hal/commit/fa7c9275b420e08823f931e59290c69a912bd50c))
    - Add the required synchronisation delays ([`067f139`](https://github.com/winksaville/rp-hal/commit/067f1396d9acf69e02abff58f994b0c980811ea3))
    - Merge pull request #399 from jannic/issue_390 ([`96552b2`](https://github.com/winksaville/rp-hal/commit/96552b28c56070322e9583082f0af514ad9e91f8))
    - Fix handling of duty cycle while PWM channels is disabled ([`c0c72c4`](https://github.com/winksaville/rp-hal/commit/c0c72c4db3d3ef2325341345e8c95c4ed4da261e))
    - Update examples to defmt 0.3 ([`46110c0`](https://github.com/winksaville/rp-hal/commit/46110c0d320ffa55f6d65514ebd8791d957ac999))
    - Merge pull request #394 from jannic/use-ref-for-clock-to-herz ([`32411b8`](https://github.com/winksaville/rp-hal/commit/32411b8652d8ffc152d89a21e56fc821d958e4aa))
    - I2c is driven from system_clock, noch peripheral_clock. Update example accordingly. ([`595e0a9`](https://github.com/winksaville/rp-hal/commit/595e0a9974d3d998a7d765fcfbed2f0eaf5be9a1))
    - Implement conversion from Clock to Hertz using reference ([`f8984a9`](https://github.com/winksaville/rp-hal/commit/f8984a9eacac19df880d7784f92d290184f68d56))
    - Merge pull request #381 from 9names/adafruit_macropad_fix_speaker_pin ([`7d11e2f`](https://github.com/winksaville/rp-hal/commit/7d11e2f15e8d2d1635f27687210c8a4696240cbe))
    - Fix incorrect pin for speaker ([`5e4805a`](https://github.com/winksaville/rp-hal/commit/5e4805ab2cd83056d250a6a76f739fd70c2f82c4))
    - Merge pull request #372 from 9names/fix_bsp_pins_docs ([`3c4d8f0`](https://github.com/winksaville/rp-hal/commit/3c4d8f0b43461a806eefdbd79d721512e8c729d3))
    - Fix unmatched parens in bsp_pins doc macro ([`319c174`](https://github.com/winksaville/rp-hal/commit/319c1749fcfe96032fff683ee24b481bdd5a4045))
    - Merge pull request #311 from Liamolucko/multicore-no-alloc ([`d66b479`](https://github.com/winksaville/rp-hal/commit/d66b47920e046f1d24336e3b34317c519aae4e35))
    - Add a fence after writing the arguments to the stack ([`e9534ac`](https://github.com/winksaville/rp-hal/commit/e9534ace04661aa0a86f7fdbcc487c175c1838ee))
    - Merge pull request #324 from 9names/bsp_use_hal_entry_macro ([`895bae9`](https://github.com/winksaville/rp-hal/commit/895bae90b56b8c1c1dd757dd88023d8caa90210f))
    - Write core 1 arguments directly to RAM without casting to usize ([`9848f84`](https://github.com/winksaville/rp-hal/commit/9848f849bd5faeea8b01a5c68b59eeccf112ec1d))
    - Set device_class of twitchy_mouse example to 0 ([`db1b5d3`](https://github.com/winksaville/rp-hal/commit/db1b5d36b579026e5b531df6d6939feeaec827a3))
    - Merge branch 'main' into main ([`f4abf18`](https://github.com/winksaville/rp-hal/commit/f4abf18be5f1562dd3ccfcf9bee0c9c2eb59dd27))
    - Fix example ([`0e5fdcf`](https://github.com/winksaville/rp-hal/commit/0e5fdcfd9cbdd0efbf4af1315366a5b4c2e17b10))
    - Add `multicore_polyblink` example ([`3e1e762`](https://github.com/winksaville/rp-hal/commit/3e1e762d20c33176655f8ed949b3d1a3d7c2d356))
    - Make `Multicore` take `SioFifo` rather than the whole `Sio` & make the `spawn` closure the last argument ([`c0fafc7`](https://github.com/winksaville/rp-hal/commit/c0fafc76940ea0a7470f9e24a09f8c987345224f))
    - Merge branch 'main' into multicore-no-alloc ([`b932663`](https://github.com/winksaville/rp-hal/commit/b932663cc9b1af7fc614e3c31d47e9e986bb4994))
    - Fix typo in rp2040-hal README.md ([`8937191`](https://github.com/winksaville/rp-hal/commit/89371912adc7ebd7886ac345de315555ac6e7003))
    - Fixed typos ([`623457a`](https://github.com/winksaville/rp-hal/commit/623457a498d3d3d612300cf48912fdd09d7ddffb))
    - Add adafruit-macropad_blinky example ([`5f793cd`](https://github.com/winksaville/rp-hal/commit/5f793cde696f05421f73dbfe5b9cc78971a58e64))
    - Abstract alarms ([`bb07402`](https://github.com/winksaville/rp-hal/commit/bb07402fc91e24a88b3aef38e9ab8e22a5ecdfa7))
    - Remove unmaintained implementation async i2c. ([`977bc27`](https://github.com/winksaville/rp-hal/commit/977bc2732a5871cb5c09bf6842de6a016cf1c9b6))
    - Update rtic example to reset spinlocks in init ([`e9a4f7e`](https://github.com/winksaville/rp-hal/commit/e9a4f7e40b46f28f4dab29406a3d9bd342eb59a9))
    - Provide an unsafe function for resetting all spinlocks ([`3d8f66d`](https://github.com/winksaville/rp-hal/commit/3d8f66df788b0dad5740936cdc0f7bc5edef96b3))
    - Merge pull request #299 from Sizurka/divider-global-asm ([`ed0cda5`](https://github.com/winksaville/rp-hal/commit/ed0cda5269ed18d8bac1e45e8c3ff1b7a4f59d37))
    - Update documentation and drop entrypoint on error ([`67ceb65`](https://github.com/winksaville/rp-hal/commit/67ceb65703d73d81c3a27945a49703534c1c25f2))
    - Remove the multicore trampoline and make the core 1 startup function generic ([`8a261b0`](https://github.com/winksaville/rp-hal/commit/8a261b050ca6ff7adba01c56e98a9d4b8b8823ac))
    - Use direct assembler calls for the divider ([`f9d2610`](https://github.com/winksaville/rp-hal/commit/f9d2610fff381b44f3358a709188d657f2f11457))
    - Change hardware divider results structure order ([`a15c109`](https://github.com/winksaville/rp-hal/commit/a15c109e8da2ae69dc138aafe0f10d16d341c38e))
    - Generate intrinsic aliases directly ([`b8ef969`](https://github.com/winksaville/rp-hal/commit/b8ef969d927e9f85746d1ec3092c3c0b69482c1a))
    - Update all BSP examples to use the BSP's re-exported entry macro ([`12cbab9`](https://github.com/winksaville/rp-hal/commit/12cbab967cc342ebd55bc57c9d1b0972c610f9ef))
    - Update BSPs to use rp2040_hal::entry instead of cortex_m_rt::entry ([`f38847a`](https://github.com/winksaville/rp-hal/commit/f38847a318c0c09dd0f1e5e7b514d1a2b1fc87d1))
    - Don't assume `usize` is 32 bits ([`56aa967`](https://github.com/winksaville/rp-hal/commit/56aa96769d0f146d4d8bac4fab28ca9640ee832b))
    - Fmt ([`51cd52b`](https://github.com/winksaville/rp-hal/commit/51cd52bb8c70e872134e9a11d0b057449f8b4448))
    - Remove the alloc requirement for `Core::spawn` ([`f0b46c0`](https://github.com/winksaville/rp-hal/commit/f0b46c0f58e5dece6963b753b098751de5046d67))
    - Fixed broken link in rp-pico Cargo.toml ([`da2372b`](https://github.com/winksaville/rp-hal/commit/da2372b19cff52b362ced933691f3b91a0678b04))
    - Merge pull request #291 from jannic/avoid-64bit-division ([`111654f`](https://github.com/winksaville/rp-hal/commit/111654fc28bcc7ef023ee2c2c3ada42283116e0b))
    - Fix clippy warnings ([`021e942`](https://github.com/winksaville/rp-hal/commit/021e942e47dd2db7e9a9079dbe176dbebccf53d7))
    - Actually run fractional_div test case from CI ([`00b49d5`](https://github.com/winksaville/rp-hal/commit/00b49d52b503fe48871d9f8a3ed3ca85c3d58a14))
    - Add test cases for fractional_div() ([`b46ddd7`](https://github.com/winksaville/rp-hal/commit/b46ddd735177186647d4d3843e4d3553b5611691))
    - Derive several traits for ClockError ([`fecde70`](https://github.com/winksaville/rp-hal/commit/fecde70cf96550fe7bcba751cb16676b8a253969))
    - Use u32 instead of u64 division in clock calculations ([`402b7f1`](https://github.com/winksaville/rp-hal/commit/402b7f1eb8c8477837b0b7d1803e0d0d497a9ce0))
    - Added so stopped PIO state machines can change their clock divider ([`b7e56d0`](https://github.com/winksaville/rp-hal/commit/b7e56d0869de0136625eff9885d6ebe809fbe9ec))
    - Merge pull request #294 from 9names/gpio_irq_example ([`212ffec`](https://github.com/winksaville/rp-hal/commit/212ffec6cadc764e464e0b66bd027cb08404e5b9))
    - Merge pull request #272 from 9names/watchdog_fix ([`4075f81`](https://github.com/winksaville/rp-hal/commit/4075f81b2d49f23d09982b54157f35e33333c12f))
    - Add note about #[interrupt] mut -> &mut transform ([`8063882`](https://github.com/winksaville/rp-hal/commit/8063882801dcdf3aa099ea512c9a73adc5cb3e79))
    - Store pins together in a tuple to reduce boilerplate ([`35875c8`](https://github.com/winksaville/rp-hal/commit/35875c875663ec171d9fe9ed43ef6c93271e4032))
    - Add GPIO interrupt example ([`44a9b0f`](https://github.com/winksaville/rp-hal/commit/44a9b0f541aa3c184faaf79c91e1d3de2bf011fb))
    - Merge pull request #290 from PavanKumarPothula/main ([`78cad0d`](https://github.com/winksaville/rp-hal/commit/78cad0df97473a6c3ba4cd13e5b02c596412fdd5))
    - Merge pull request #289 from astraw/fix-typo ([`fff9806`](https://github.com/winksaville/rp-hal/commit/fff980611a2cae3852700140feec9deb03a30f55))
    - Merge pull request #288 from Sizurka/rom-intrinsics ([`f46c23d`](https://github.com/winksaville/rp-hal/commit/f46c23d3b74bbacdb749d83a32d953bbd90497d6))
    - Add ROM floating point math library ([`80c84b1`](https://github.com/winksaville/rp-hal/commit/80c84b13bad87c0015d17132ae8656ea0cbfcded))
    - Move divider intrinsics to the new intrinsics macro ([`ce681b4`](https://github.com/winksaville/rp-hal/commit/ce681b4f101e15ecafcfef5e385ed0715a3278fb))
    - Add basic ROM intrinsics ([`a70eb89`](https://github.com/winksaville/rp-hal/commit/a70eb89799dfe0861344ef9b0aca7991b2a71605))
    - Just a typo in the hyperlink. Nothing much. ([`438ffcc`](https://github.com/winksaville/rp-hal/commit/438ffccf698611010bee00c54b73c0bdf17ee49e))
    - Add ROM version check ([`81ab38f`](https://github.com/winksaville/rp-hal/commit/81ab38fd7178407adf95b5c289461276e3d20e3e))
    - Fix typo ([`799449d`](https://github.com/winksaville/rp-hal/commit/799449dd1ae77745af598cff29cd7f63b858bef3))
    - Fix ROM function signatures ([`a6f2453`](https://github.com/winksaville/rp-hal/commit/a6f245344072b59e5b7e5830efcf5bde07e74ee9))
    - Merge pull request #283 from Sizurka/rom-functions ([`8bdecd2`](https://github.com/winksaville/rp-hal/commit/8bdecd20589dd9242b18fe1f7627cb96a1e4ea99))
    - Add ROM function caching ([`98fd6c1`](https://github.com/winksaville/rp-hal/commit/98fd6c1724e3fbea60940d67e57567e2e98df598))
    - Standardize ROM function access ([`a6daaf9`](https://github.com/winksaville/rp-hal/commit/a6daaf9fa33715c9a311a612591687791334b7e7))
    - Merge pull request #280 from 9names/alarm-ergonomics ([`16c9064`](https://github.com/winksaville/rp-hal/commit/16c9064c529fb977816b3f96aa3e549c2b5ba339))
    - Merge pull request #278 from Sizurka/divider-intrinsics ([`385c923`](https://github.com/winksaville/rp-hal/commit/385c92392bb3bef992271834f54b08dfbe29934d))
    - Merge pull request #285 from astraw/pio-side-set-example ([`1a58449`](https://github.com/winksaville/rp-hal/commit/1a58449cf4d7e313c364cc59b7c6448b41670698))
    - Run 'cargo fmt' ([`cd15d26`](https://github.com/winksaville/rp-hal/commit/cd15d268f69aa367ac1943af1c54472d43baa9e4))
    - Example of side setting using PIO ([`a1ed9ef`](https://github.com/winksaville/rp-hal/commit/a1ed9ef93c8b81b17003bb1e6f0593b3d35f7c4c))
    - Merge pull request #281 from rp-rs/update_pac ([`354a2a5`](https://github.com/winksaville/rp-hal/commit/354a2a5e5e1c72103d1d80b1374bbc9b5281ccaa))
    - Merge pull request #279 from jannic/dht11_example ([`baff438`](https://github.com/winksaville/rp-hal/commit/baff438f537c94bfcffa0231a03680c4df253161))
    - Hide spinlock 31. ([`4a540d0`](https://github.com/winksaville/rp-hal/commit/4a540d041abf60c61ec93180946be995f2cfecac))
    - Update spinlock docs. ([`efda22c`](https://github.com/winksaville/rp-hal/commit/efda22c9eac0ee14a3c4c48cc7e9fe0bcba24700))
    - Make clippy happy. ([`f44f5f0`](https://github.com/winksaville/rp-hal/commit/f44f5f0e09d8be39c929e9477f1cc56f8a795888))
    - Clean up critical-section impl. ([`35a10f2`](https://github.com/winksaville/rp-hal/commit/35a10f2bc69384566ce72538f60ddb88174a60c3))
    - Use const generics for spinlocks. ([`7e2f8d2`](https://github.com/winksaville/rp-hal/commit/7e2f8d274cb2de434bc1730600f0fd49f581ac67))
    - Use new spinlock API provide by PAC 0.3.0 ([`c8c366c`](https://github.com/winksaville/rp-hal/commit/c8c366c23dcc9a49af932e16b835282f09dfa166))
    - Use new alarm syntax in pico_rtic example ([`f51a84f`](https://github.com/winksaville/rp-hal/commit/f51a84f0701b5fe4b78ee14828feef88d64aaaa7))
    - Use atomic operations for altering Timer interrupts ([`b19f2cc`](https://github.com/winksaville/rp-hal/commit/b19f2cc8e579c0e28308c613a9331a4d6a8d992d))
    - Add comment regarding release mode ([`a976383`](https://github.com/winksaville/rp-hal/commit/a9763837a90bf4497a21c95bda42531bbec208a1))
    - Use dht-sensor crate and fix comments ([`f6b2e33`](https://github.com/winksaville/rp-hal/commit/f6b2e3365ec886bbac5cc42a82ef3eee816f8f5e))
    - Add dht11 example ([`bb6b770`](https://github.com/winksaville/rp-hal/commit/bb6b7706f96d788fd635ec81244118f08762efe5))
    - Merge pull request #269 from 9names/fix_uart_example_clock ([`5771f87`](https://github.com/winksaville/rp-hal/commit/5771f872f2d08af821ea405d09d12e3d404996b5))
    - Fix i2c peripheral mode state machine ([`d08bfac`](https://github.com/winksaville/rp-hal/commit/d08bfac989c43bece7c4350946f9b4c1e06a4a47))
    - Fix View Demos link by prefixing `pico` with `rp-` ([`d6bb177`](https://github.com/winksaville/rp-hal/commit/d6bb177fd79374213d4bb667431f8b73fcbd2b03))
    - Add intrinsics for the hardware divider ([`f279945`](https://github.com/winksaville/rp-hal/commit/f279945315546592ac98076c498fe720b3005889))
    - Change divider delay to explicit NOPs ([`35704d9`](https://github.com/winksaville/rp-hal/commit/35704d97991edc153edafe05e2b562e2c7494138))
    - Make hardware divisor interrupt safe ([`c2d3b21`](https://github.com/winksaville/rp-hal/commit/c2d3b21d91dae55280e367a7d45f2c8c10336fb6))
    - Merge pull request #271 from 9names/kb2040-boot2 ([`c180e78`](https://github.com/winksaville/rp-hal/commit/c180e7867b9463793c993a05e792c8ffb690d870))
    - Set hw reset bits for watchdog ([`57e9943`](https://github.com/winksaville/rp-hal/commit/57e99438360ff3df85d0569d0515dff250fb2f43))
    - Make boot2 optional ([`8b7b0b1`](https://github.com/winksaville/rp-hal/commit/8b7b0b168bbfbf2d23985dff4c86c6efe62a234f))
    - Add boot2 feature to kb2040 BSP ([`332fe64`](https://github.com/winksaville/rp-hal/commit/332fe645a8ef2f9171bcab822fcd8a8cc71339fd))
    - Use .freq() to avoid moving clock ([`c8b7520`](https://github.com/winksaville/rp-hal/commit/c8b75204ee5df29549d79768790995335ac807de))
    - Merge pull request #268 from VictorKoenders/default-uart-config ([`3a0e23c`](https://github.com/winksaville/rp-hal/commit/3a0e23c406a650c52c4e8972c7df356bc5296dfc))
    - Set the uart config default baud rate to 115200 ([`d6e3c7b`](https://github.com/winksaville/rp-hal/commit/d6e3c7b61567ade03e492ee8bc7b58c61406c1de))
    - Fixed doc test ([`b3b4d9f`](https://github.com/winksaville/rp-hal/commit/b3b4d9ff6fcf9b217b071f4052ec8d419a56be0d))
    - Added `impl Default` for UartConfig ([`9e75cec`](https://github.com/winksaville/rp-hal/commit/9e75cec551429719da2f84b2f40eeaaecbf7f3cd))
    - Merge pull request #266 from dylanede/feature/qt2040 ([`bae3f2c`](https://github.com/winksaville/rp-hal/commit/bae3f2c9bc2a5b6e95af55122441ab115f1d4153))
    - Board support for Adafruit Trinkey QT2040 ([`6478917`](https://github.com/winksaville/rp-hal/commit/6478917e5160c23314ffade9d5d2fbe6c775608d))
    - Merge pull request #267 from rp-rs/add_stamp_to_readme ([`7525040`](https://github.com/winksaville/rp-hal/commit/7525040c1b5dbfc2765ace4bbbf85d0bc6fc0a37))
    - Add missing Solder Party Stamp to top README - ([`a8b84fa`](https://github.com/winksaville/rp-hal/commit/a8b84fa4f8b61554074fc2d9c2a92a334c855bcb))
    - Fix unexpected restart on repeated read. ([`7840d0f`](https://github.com/winksaville/rp-hal/commit/7840d0f8333d7a9a6dd0f07389d1d73c11caf97b))
    - Merge pull request #264 from WeirdConstructor/pico_i2c_oled_text_display_ssd1306_example ([`ce7c9f4`](https://github.com/winksaville/rp-hal/commit/ce7c9f4be31e795465a7ace9fd95e85a17d810f2))
    - Cleaned up the code and made it more idiomatic. ([`3f9535c`](https://github.com/winksaville/rp-hal/commit/3f9535cc1fd4c70f20790a4c92f3613c77d17b21))
    - Merge pull request #263 from WeirdConstructor/fix_alarm_schedule_race_cond ([`d3c9c3b`](https://github.com/winksaville/rp-hal/commit/d3c9c3b4e2ce65d3e05da51f7f5ed48b0dd34801))
    - Merge pull request #259 from WeirdConstructor/pico_board_documentation ([`f7b8abf`](https://github.com/winksaville/rp-hal/commit/f7b8abfeb0645d8c7f490738899ed4ec90e79466))
    - Mention the assumed display size of 128x64. ([`e22540b`](https://github.com/winksaville/rp-hal/commit/e22540be20a4e3d296c49f6dff1799ae4e6ed03f))
    - Added documentation for the OLED example and fixed formatting. ([`2f1e77d`](https://github.com/winksaville/rp-hal/commit/2f1e77d0b28578c977e04e492ba2d1320d0b65b4))
    - Add an example for using the SSD1306 I2C display driver crate with the Raspberry Pi Pico ([`2f418bb`](https://github.com/winksaville/rp-hal/commit/2f418bbf8fef99fbb7f6af1ac29788b72b2a2291))
    - Merge branch 'rp-rs:main' into fix_alarm_schedule_race_cond ([`fdc36d3`](https://github.com/winksaville/rp-hal/commit/fdc36d30cc17f91d228e9a40401288a25bd16ef3))
    - Fix alarm schedule() race condition. ([`7a23247`](https://github.com/winksaville/rp-hal/commit/7a23247ca11b6329bf43a5c810905f6feecdbce4))
    - Merge pull request #261 from jkristell/solderparty-stamp ([`0cb171f`](https://github.com/winksaville/rp-hal/commit/0cb171ffc8fae347c0f80fbc0a087921d35e659a))
    - Merge pull request #260 from WeirdConstructor/pico_ws2812_led_example ([`7a86e7d`](https://github.com/winksaville/rp-hal/commit/7a86e7d6382242e0163bda1a3d5e3e57500da5a0))
    - Formatted the tables in the comments properly. ([`0b31054`](https://github.com/winksaville/rp-hal/commit/0b3105442990368d24878e8f11a758e09281d3d2))
    - Removed weird rom function usage, reformulated comments and cleaned up hsv2rgb() code. ([`5b07c09`](https://github.com/winksaville/rp-hal/commit/5b07c09cfbe1bfbe4bde4fd754b6694daa99ebd2))
    - Add Solder Party RP2040 Stamp board ([`21a4fde`](https://github.com/winksaville/rp-hal/commit/21a4fde0c87383c14095b5f9a58bc347475da249))
    - Add Raspberry Pi Pico WS2812 LED example ([`2b49bc6`](https://github.com/winksaville/rp-hal/commit/2b49bc6b604548270a424228053aa6a67d8df0f6))
    - Fix compilation bug in the documentation ([`a7b71bd`](https://github.com/winksaville/rp-hal/commit/a7b71bd5aa5fd8143801dd1bd8ac6a7186ad8768))
    - Improved the rp_pico pin documentation with aliases, table and cross links. ([`adfe63f`](https://github.com/winksaville/rp-hal/commit/adfe63f0df266d120f83e5c442dfa316930bdf80))
    - (Hopefully) Improved documentation of bsp_pins!() ([`9e84c96`](https://github.com/winksaville/rp-hal/commit/9e84c961a8f65ddc7a4d3169a5f0f18febcfb97e))
    - Remove trailing spaces ([`f4a4b80`](https://github.com/winksaville/rp-hal/commit/f4a4b80459a74524834e1c380f8a9b7e6f4a85b9))
    - Added pin function documentation from the datasheet to rp-pico ([`160099b`](https://github.com/winksaville/rp-hal/commit/160099b6d8b208259f267380f89326f5bbf06128))
    - Merge pull request #254 from 9names/fix_ci_masking_link_errors ([`8d18abd`](https://github.com/winksaville/rp-hal/commit/8d18abdfc7c0129debba85457d32d32175bf36bd))
    - List examples built as well ([`eddf3dc`](https://github.com/winksaville/rp-hal/commit/eddf3dc0d4daeccbea1ff71c25cec244349106ca))
    - Merge pull request #197 from chinoto/pio_sound_send ([`f23abab`](https://github.com/winksaville/rp-hal/commit/f23ababb1af1ed34231b614550307c7eb3d3617c))
    - Do release builds for examples as well ([`8b9028d`](https://github.com/winksaville/rp-hal/commit/8b9028d97f5c46033a683aada8d1ad14a158ce8c))
    - Do cargo build instead of cargo check so we test linking ([`20954f2`](https://github.com/winksaville/rp-hal/commit/20954f2240272112b4a6234c624216b58116323d))
    - Unmask rustc/ld warnings, remove deprecated '--all' ([`f60828c`](https://github.com/winksaville/rp-hal/commit/f60828c9a4645414c916852ce3b877df1a317803))
    - Merge pull request #255 from 9names/fix_boot2_in_examples ([`78176de`](https://github.com/winksaville/rp-hal/commit/78176deffca41e3653ec60bd6333f76b6498351b))
    - Remove static BOOT2 decl in BSP examples so they build ([`0e1fe81`](https://github.com/winksaville/rp-hal/commit/0e1fe81384fa705b337462f27d677da45f035069))
    - Remove mention of boot select button ([`c02984b`](https://github.com/winksaville/rp-hal/commit/c02984b422d3cc12e14a3e17373f7bb3b57e5e58))
    - Merge pull request #248 from jannic/bump-versions ([`43650b3`](https://github.com/winksaville/rp-hal/commit/43650b3248a67c4e9cdac384b03464d6be82feec))
    - Merge pull request #247 from rp-rs/uart_irq_example ([`3c2d503`](https://github.com/winksaville/rp-hal/commit/3c2d5038448dca503e3c29d84178a9eadc442aba))
    - Merge pull request #249 from rp-rs/fix-readme-links ([`ac133ac`](https://github.com/winksaville/rp-hal/commit/ac133acb0278831424b5fff6cce6dc7be16717f1))
    - Fix docs for SerialInfallible. ([`67d9da8`](https://github.com/winksaville/rp-hal/commit/67d9da85e6eb796d2862915897c52679816dc571))
    - Fix build errors in eh_1.0 mode. ([`55acbdb`](https://github.com/winksaville/rp-hal/commit/55acbdb1b0b6d757f9a107c51c7ddf13a1c9c70c))
    - Fix the links in README.md ([`232ba73`](https://github.com/winksaville/rp-hal/commit/232ba734fa6d6e10441bf0e85d326fecd233d2e4))
    - Bump versions of HAL and BSPs ([`2f9a950`](https://github.com/winksaville/rp-hal/commit/2f9a950cbea0df57c797a2e0c23b76cd686d8ee0))
    - Fixing typos spotted in the review. ([`7da16a7`](https://github.com/winksaville/rp-hal/commit/7da16a726fdd121911605bd0ab4d383d7b137cd8))
    - Added two UART IRQ examples. ([`d3bd232`](https://github.com/winksaville/rp-hal/commit/d3bd232885c9e8a1c4f1a5bb7391fee1f89a351d))
    - Merge pull request #210 from VictorKoenders/uart-owning-pins ([`cc53c17`](https://github.com/winksaville/rp-hal/commit/cc53c1777f0d94e135660b299b80ad93270e6db8))
    - Fixed failing doctest ([`8f63be0`](https://github.com/winksaville/rp-hal/commit/8f63be0f22275e12e15bcf483a661aa300d1418b))
    - Migrated examples to the new uart system ([`8644444`](https://github.com/winksaville/rp-hal/commit/86444448a4422101c0e0bd3c4fbd5bbd0dc42d14))
    - Added reader/writer split to UartPeripheral ([`c41c273`](https://github.com/winksaville/rp-hal/commit/c41c27313193295506966a60c0fb12513f8ceed1))
    - Fixed compile errors on eh1_0_alpha feature ([`84b8fb0`](https://github.com/winksaville/rp-hal/commit/84b8fb05b032df985194f346ab7e60f5e7d05cf7))
    - Constraint the uart::pin:: traits to UartDevice ([`a8a2767`](https://github.com/winksaville/rp-hal/commit/a8a27672b8d0d4092fa559612008069a30b1f69c))
    - Added pins to the uart constructor functions ([`a4a0bcf`](https://github.com/winksaville/rp-hal/commit/a4a0bcf9876fcf85d57ab95c1c891fed4cbb5653))
    - Split uart in separate files, introduced a typesystem constraint for valid UART pin configurations ([`bdfb4d8`](https://github.com/winksaville/rp-hal/commit/bdfb4d82c9c9d1d2f9f23c45f4d03132e7f2b962))
    - Fix KB2040/adafruit-kb2040 mix-up in README. ([`3eb6516`](https://github.com/winksaville/rp-hal/commit/3eb65168ffb7c97f893e757a3bd982fd0446c6f7))
    - Merge pull request #245 from rp-rs/clean-up-bsp ([`882d91c`](https://github.com/winksaville/rp-hal/commit/882d91cd276337b9cb9eaae7283fda795ec5e567))
    - Rp-pico will be 0.2.0 as 0.1.0 exists already. ([`6271e86`](https://github.com/winksaville/rp-hal/commit/6271e8670fe61cafb48f636ceaf5e001949a1442))
    - Renamed pico to rp-pico. ([`8f0a278`](https://github.com/winksaville/rp-hal/commit/8f0a2788eb05813f61c38eb502fc88b5bba749b7))
    - Formatting ([`882868c`](https://github.com/winksaville/rp-hal/commit/882868c1048d67cd2e585831c01b8bca0e6040d6))
    - Include manufacturer in BSP crate name. ([`4959afe`](https://github.com/winksaville/rp-hal/commit/4959afe151ce14b083be0854caeaef3e66b4da21))
    - Update all the BSPs. ([`37e7d2e`](https://github.com/winksaville/rp-hal/commit/37e7d2e7b65828364d922c939cfcab21ec5da32d))
    - Merge pull request #243 from rp-rs/release_030 ([`c83a31a`](https://github.com/winksaville/rp-hal/commit/c83a31ab2b52b7af55e045fd570aeab3f8c31da7))
    - Add MSRV ([`7278c36`](https://github.com/winksaville/rp-hal/commit/7278c36e93d7d8e62523ce170cb7528470b4a9d0))
    - Noted 0.3.0 includes many bug fixes. ([`96c2273`](https://github.com/winksaville/rp-hal/commit/96c2273dce9d2e41599a3492d5fb0edcf129d9f6))
    - Revised CHANGELOG. ([`5701ab4`](https://github.com/winksaville/rp-hal/commit/5701ab431f966062fba4c2382b3bd5b81fc87d57))
    - Set up for 0.3.0 release. ([`bebf85d`](https://github.com/winksaville/rp-hal/commit/bebf85d4d9ec829e4f98b282dd9c15922401d259))
    - Merge pull request #242 from rp-rs/remove-embassy ([`e6d19bc`](https://github.com/winksaville/rp-hal/commit/e6d19bc59b7df162f0be8743e99f932d8f8f1806))
    - Comment out embassy traits. ([`a9f6ab8`](https://github.com/winksaville/rp-hal/commit/a9f6ab8de462242cd4e23a6dc3102e01aca1b54f))
    - Merge pull request #235 from camrbuss/rtic-timer-hal ([`31285fe`](https://github.com/winksaville/rp-hal/commit/31285fe00277fa4e52f036014a6599df7f8b74c6))
    - Pico bsp hal pac ([`546ad37`](https://github.com/winksaville/rp-hal/commit/546ad3799be54f4f67532c4f7aea9d1940228675))
    - Update pico rtic example to use timer alarm hal ([`f2f50d0`](https://github.com/winksaville/rp-hal/commit/f2f50d0fc3770ae4b6509a282dac26369ebc74a5))
    - Merge pull request #231 from ithinuel/bump-embassy ([`539f6db`](https://github.com/winksaville/rp-hal/commit/539f6db0f7999578496c0253cd69dccb3a945433))
    - Merge pull request #232 from jannic/refactor-uart-init ([`b94a5ab`](https://github.com/winksaville/rp-hal/commit/b94a5ab88566b4b5e3e0a019b0f2ba04c1ab9d79))
    - Merge pull request #227 from 9names/reexport_mod_structs ([`e64f307`](https://github.com/winksaville/rp-hal/commit/e64f307d4798fcf1dcacfbcc002e990cef417b87))
    - Bump embassy's dependencies ([`fee8881`](https://github.com/winksaville/rp-hal/commit/fee8881801b3bc3df064d1904a4fd4e798f27256))
    - Bump i2c_pio to an API with better inference. ([`b363038`](https://github.com/winksaville/rp-hal/commit/b3630384778c4eb5ebf32db5758cef725bbd02bc))
    - Reset UART in new() ([`b380b3d`](https://github.com/winksaville/rp-hal/commit/b380b3ddf69a78269ca6409e6d376a2c7b5a37b6))
    - Merge branch 'main' into reexport_mod_structs ([`422da14`](https://github.com/winksaville/rp-hal/commit/422da14e1916371f12d986328cfc53a3e96ec896))
    - Merge pull request #228 from rp-rs/fix-readme-picoprobe ([`88bd408`](https://github.com/winksaville/rp-hal/commit/88bd408bc1ea46128918877435a9c716726f75ca))
    - Replace rp2040_hal::pio::PIOExt with bsp::hal::pio::PIOExt in BSPs ([`978f846`](https://github.com/winksaville/rp-hal/commit/978f84680528f1476ff693e9c63d2b04bf558d73))
    - Fix picoprobe/picotool mix up ([`3f0617b`](https://github.com/winksaville/rp-hal/commit/3f0617b05476f30124a665a6d4f017d4634d9775))
    - Replace hal::timer::Timer with hal::Timer or Timer ([`6e184a9`](https://github.com/winksaville/rp-hal/commit/6e184a91a785e9119c0a14b90c52f351bceb1593))
    - Replace uses of hal::watchdog::Watchdog with hal::Watchdog ([`def0ed9`](https://github.com/winksaville/rp-hal/commit/def0ed97f720365f6b5fe9b8962c51e446b43bd2))
    - Move uses of sio::Sio to Sio ([`dc8ceff`](https://github.com/winksaville/rp-hal/commit/dc8ceffd09e2554d1b17477c783c84a60ac6b136))
    - Cargo fmt ([`11aa0b8`](https://github.com/winksaville/rp-hal/commit/11aa0b87af05215dcb0e68565ddc6620e05468d9))
    - Refactor Uart initialization ([`26fa532`](https://github.com/winksaville/rp-hal/commit/26fa532fa34f9b7a261a78001a804280a009b37f))
    - Merge branch 'rp-rs:main' into reexport_mod_structs ([`33ff337`](https://github.com/winksaville/rp-hal/commit/33ff337631b3780fda98d2b3299a5dffaadbef98))
    - Generate sev in sio.fifo.write() ([`6ab9cd7`](https://github.com/winksaville/rp-hal/commit/6ab9cd7ed3dbb2a1a9fe7ab1cf043a4802b7483b))
    - Re-export mod structs ([`55a8b4a`](https://github.com/winksaville/rp-hal/commit/55a8b4acf9b81f3e40c23e821662da7f3786e6e6))
    - Add safety docs from atsamd-rs to GPIO traits ([`a7d5dc2`](https://github.com/winksaville/rp-hal/commit/a7d5dc2bee2274255acd714155f8973ad6ca2d2b))
    - Use user-provided stack for core 1 ([`5dafe39`](https://github.com/winksaville/rp-hal/commit/5dafe3985f634ed18783096a158c04b7912afb22))
    - Handle errors of serial.write() ([`de53600`](https://github.com/winksaville/rp-hal/commit/de536001995c07f9abf8026a72ed140aa0f08df1))
    - Change references to probe-run-rp back to upstream probe-run ([`05e0720`](https://github.com/winksaville/rp-hal/commit/05e072025d00239fc49734e203bf39282b53cb2d))
    - Merge pull request #191 from jannic/rename-set_instruction ([`fad1dfa`](https://github.com/winksaville/rp-hal/commit/fad1dfa259ccaa69ce16e99ec8779234aecf84d4))
    - Merge pull request #204 from rp-rs/add_sio_fifo ([`3a32805`](https://github.com/winksaville/rp-hal/commit/3a3280575f530311e8f9f71cff714569d6a0db65))
    - Fix fmt ([`bb85314`](https://github.com/winksaville/rp-hal/commit/bb8531445ea0eed74cc77b9bd37c877207279514))
    - Update docs in rp2040-hal/src/pio.rs ([`15c1627`](https://github.com/winksaville/rp-hal/commit/15c162757f23ce0f0e91bc2b3fd790a07dc7cc4d))
    - Fix wfe/sev semantics. ([`69255f7`](https://github.com/winksaville/rp-hal/commit/69255f7b8c92b7c3c402e730f77f0fb3d0d3df34))
    - Use released 0.2.0 PAC. ([`e9694bb`](https://github.com/winksaville/rp-hal/commit/e9694bbb91c66e67df7150fa900a82d9fad928ff))
    - Merge pull request #208 from VictorKoenders/spinlock ([`ed860ed`](https://github.com/winksaville/rp-hal/commit/ed860ed106545f28ec81dd8574cccc34c8bf5359))
    - Merge pull request #198 from VictorKoenders/alarm ([`968e49a`](https://github.com/winksaville/rp-hal/commit/968e49aa03949916cd412205134b1e6bc1b4b906))
    - Merge pull request #205 from jannic/eh-1_alpha6 ([`292a6f1`](https://github.com/winksaville/rp-hal/commit/292a6f13c8ed763674b9115c677b65b3804cf22e))
    - Fixed error in spinlock's documentation ([`111b355`](https://github.com/winksaville/rp-hal/commit/111b355da28b1af14c138930166f443287ab3dfc))
    - Added spinlocks ([`88fbc38`](https://github.com/winksaville/rp-hal/commit/88fbc38f8b973c6c40c4d82248a831571fbe753b))
    - Removed incorret unsafe impl Sync, added interrupt_free around obtaining an alarm ([`a9d96f3`](https://github.com/winksaville/rp-hal/commit/a9d96f352e8f180a269f70a47e43ff7330faffaa))
    - Made the alarmX take exclusive ownership of Timer on functions that could cause UB when run in parallel ([`1fd04d3`](https://github.com/winksaville/rp-hal/commit/1fd04d3384395228e9fe4daba8a8c90680e4c96c))
    - Added AlarmX::disable_interrupt, made AlarmX::schedule able to return an error if the time is too short ([`97a5bd3`](https://github.com/winksaville/rp-hal/commit/97a5bd355cc519c20c46c99ae88646de70527cd7))
    - Added timer alarms ([`119c5a9`](https://github.com/winksaville/rp-hal/commit/119c5a94e822eb729d2bef63bf53cb2c07b9ae33))
    - Merge pull request #199 from ithinuel/simplify-types ([`4fb005f`](https://github.com/winksaville/rp-hal/commit/4fb005f5b671fb9e93a720a6566fb45bd9fd7369))
    - Fix unsound Send clippy warning ([`c7c5fb0`](https://github.com/winksaville/rp-hal/commit/c7c5fb00d8b97d6fdcdaf66d67d5e0d85e9e580c))
    - Update comments ([`3ab8470`](https://github.com/winksaville/rp-hal/commit/3ab84702b7701c551f608e028ba6f6a6e433b5de))
    - Merge pull request #206 from rp-rs/pac_020_changes ([`8e07b2c`](https://github.com/winksaville/rp-hal/commit/8e07b2c8c21cb3fee1642da2c95de62f0378581b))
    - Update uart implementation of embedded-hal 1.x to 1.0.0-alpha.6 ([`9a018ac`](https://github.com/winksaville/rp-hal/commit/9a018ac359faee6c4c452e91a9939fb8cc8b4053))
    - Update SPI implementation of embedded-hal 1.x to 1.0.0-alpha.6 ([`1294f55`](https://github.com/winksaville/rp-hal/commit/1294f556e96fb0920fed442ecfe58dcbc944ccbe))
    - 0.1.6 had breaking changes, so I yanked it and made 0.2.0. ([`68602fa`](https://github.com/winksaville/rp-hal/commit/68602fa6e1291f82f8bcaf16b2e53301c340c3d3))
    - PAC 0.1.6 is now released. ([`84b903b`](https://github.com/winksaville/rp-hal/commit/84b903b12a498057149343ff103010fe6121ece6))
    - Update I2C implementation of embedded-hal 1.x to 1.0.0-alpha.6 ([`0f3bb8e`](https://github.com/winksaville/rp-hal/commit/0f3bb8e88c5a5e70b21dc7c5d3ed4d424405baf6))
    - Update dependency on embedded-hal 1.x to 1.0.0-alpha.6 ([`76aff05`](https://github.com/winksaville/rp-hal/commit/76aff05cec0ead25223cb6e275461e53a2080f23))
    - Apply clippy's suggestions. ([`038f792`](https://github.com/winksaville/rp-hal/commit/038f792e211bef4f61b7e979c041e8f4e531f045))
    - Add SIO FIFO interface. ([`6801446`](https://github.com/winksaville/rp-hal/commit/68014469dd8ed87715ef0eb61af9181b7838d31e))
    - Point at PAC release branch. ([`23bafb6`](https://github.com/winksaville/rp-hal/commit/23bafb6980db6ee9a60d5baf696f5ed14d8b053b))
    - Changes to work with upcoming PAC 0.16. ([`0a082c0`](https://github.com/winksaville/rp-hal/commit/0a082c0f03657312735c0bc45d884bc297869a76))
    - Merge pull request #201 from rp-rs/rename-gpio23 ([`9d56062`](https://github.com/winksaville/rp-hal/commit/9d56062e447957f7304c31cbe7153abfe70a4f28))
    - Set button as pull-up. ([`ffffa73`](https://github.com/winksaville/rp-hal/commit/ffffa7368a1dfe9bd7e8faa6348c332cfbe3d770))
    - Fix-up the examples and BSPs. ([`ac88d89`](https://github.com/winksaville/rp-hal/commit/ac88d89939adfd17b829897dfcbebd94020ea332))
    - GPIO23 actually controls the 'power save' function on the SMPS. ([`cc612b8`](https://github.com/winksaville/rp-hal/commit/cc612b89fdd34f0000fab12ba0b23a0c659194f6))
    - Merge pull request #200 from rp-rs/pio_helpers ([`1541e0d`](https://github.com/winksaville/rp-hal/commit/1541e0dfa4e85fde9fb02225a12a9ae0b641e7b6))
    - Keep old function as a deprecated alternative, for now ([`aafa3dd`](https://github.com/winksaville/rp-hal/commit/aafa3dd587611af8bc6651147cb18f4c0b016bc1))
    - Rename set_instruction to exec_instruction ([`3756cd2`](https://github.com/winksaville/rp-hal/commit/3756cd2fb5165eeb078063e0b8ec6aaca87a7b28))
    - Resolve review comments. ([`b9497d9`](https://github.com/winksaville/rp-hal/commit/b9497d9b82803a50559e6f4914e205fb1b4a258d))
    - Adds some useful functions when using PIO FIFOs with DMA. ([`5c1bcd2`](https://github.com/winksaville/rp-hal/commit/5c1bcd2604a3a40e7564392f519129ea04a5b477))
    - Bump to latest ws2812 driver's revision. ([`4ccf71a`](https://github.com/winksaville/rp-hal/commit/4ccf71a6de2e5b9b62ee6ce2b656a6d6b56091f2))
    - Add --locked to second `cargo install elf2uf2-rs` ([`3977bdd`](https://github.com/winksaville/rp-hal/commit/3977bdd8c5ddeb16de2e8df4596bad314e04960b))
    - Add methods to set and clear the PWM Interrupt force register. ([`fb69308`](https://github.com/winksaville/rp-hal/commit/fb693080581b891e36fec178890b7fb6471f0ac2))
    - Fix UART init code ([`b1dc9ae`](https://github.com/winksaville/rp-hal/commit/b1dc9aec8c0ff0dc28e70dfde3f672fc50c6bc06))
    - Make ReadableOutput public to match the visibility of other Type-level variant of PinMode. ([`73e2c69`](https://github.com/winksaville/rp-hal/commit/73e2c6921fba8783b67441382e75440923376228))
    - Merge pull request #182 from jannic/issue-181 ([`3b019fb`](https://github.com/winksaville/rp-hal/commit/3b019fb91d33be76dd0fa515f8f3c4d1628cd441))
    - Correct limit for PIOBuilder::out_pins count argument ([`9f55608`](https://github.com/winksaville/rp-hal/commit/9f55608f928c4280230a8cabfe8afdece1f92a83))
    - Mark Timer as sync ([`9707948`](https://github.com/winksaville/rp-hal/commit/97079489ef8fbf1551ad651da6c55e325617cd5b))
    - Minor docs improvements in pio.rs ([`4c4d12e`](https://github.com/winksaville/rp-hal/commit/4c4d12e23cb4b9267b773d4abd48bf1c542fa9b3))
    - Add option --locked to cargo install elf2uf2-rs ([`233f7c9`](https://github.com/winksaville/rp-hal/commit/233f7c947514b6b96ff8a146c2ddac8ac16ce510))
    - Merge pull request #171 from 42-technology-ltd/update_boot2 ([`6330dab`](https://github.com/winksaville/rp-hal/commit/6330dab44ea6d8ba508819c477b1b0b51dd096f9))
    - Ah, missed one after the rebase. ([`e48323c`](https://github.com/winksaville/rp-hal/commit/e48323c983733034f15050f1859b821aefb2d9fc))
    - Can we build without GCC now? ([`e3f9125`](https://github.com/winksaville/rp-hal/commit/e3f9125a87f8b13acc6b7c1b22cc78dcb9e4f4cc))
    - Switch to new rp2040-boot2 crate. ([`8e66ddc`](https://github.com/winksaville/rp-hal/commit/8e66ddcfb18df3c1e11775912fd9ce82eec2cd42))
    - Support zero post-divide ([`c8bb2e4`](https://github.com/winksaville/rp-hal/commit/c8bb2e43c792dd3975a255d7eba479547411aec6))
    - Merge pull request #165 from 42-technology-ltd/bootrom_functions_update ([`dd4a9a8`](https://github.com/winksaville/rp-hal/commit/dd4a9a8f22de096a44ec1c577065c02c6d477c84))
    - Formatting. ([`6a4a4fd`](https://github.com/winksaville/rp-hal/commit/6a4a4fd247a421ad7af4e1d403e7b559c78f5153))
    - Cleaning up the comment summaries. ([`74ea262`](https://github.com/winksaville/rp-hal/commit/74ea262f654633f2431018d03ce45899fb9cd6d2))
    - Clean up comments. ([`2423e42`](https://github.com/winksaville/rp-hal/commit/2423e42eb9ca3ec9f8fb25f3def9531b3567a867))
    - Typo ([`5c55af7`](https://github.com/winksaville/rp-hal/commit/5c55af76d23de229b0d26bcaf58f29c77c14a501))
    - Moved float and double functions into modules. ([`e1afb70`](https://github.com/winksaville/rp-hal/commit/e1afb70bd244b9c076c33c6821576857fc128142))
    - Tweak doc comments. ([`ae66ac4`](https://github.com/winksaville/rp-hal/commit/ae66ac4cb62da0b0803d80fbd75ccc739b1f6bab))
    - Add comment to `calc_delta` function as it's non-obvious. ([`64207a6`](https://github.com/winksaville/rp-hal/commit/64207a62e5159554d4b55cbdcbe5b7117e7d735b))
    - Add example which uses the ROM functions ([`f56369e`](https://github.com/winksaville/rp-hal/commit/f56369e1c7c90d67cf3bbe5d0e306c40c6d9c502))
    - Fix the ROM function table code. ([`7a05b8f`](https://github.com/winksaville/rp-hal/commit/7a05b8f3a75251d7ad4827a4857abbdf47164244))
    - Merge pull request #157 from 42-technology-ltd/add-cargo-config-helptext ([`02cb4b8`](https://github.com/winksaville/rp-hal/commit/02cb4b8b067ae9ab929d0ab2f1f86e588a57a704))
    - Merge pull request #147 from Lichtso/feature/gpio_interrupt ([`a0740a5`](https://github.com/winksaville/rp-hal/commit/a0740a5ac3c0aa3881eb66b23191f312db7a0e36))
    - Merge pull request #152 from anall/feature/rom_data_unsafe_reapply ([`f92c990`](https://github.com/winksaville/rp-hal/commit/f92c9900cf7e6d9aef8908397db25c7385f87ed0))
    - Make pio-proc a dev-dependency ([`e63f1f6`](https://github.com/winksaville/rp-hal/commit/e63f1f6dee0c632877944add1c895a5d2b33528a))
    - Add some help text. ([`3d8ccf5`](https://github.com/winksaville/rp-hal/commit/3d8ccf55ab12c27419220d990148391894ae1bf3))
    - Split rom_data into safe and unsafe functions ([`dab619d`](https://github.com/winksaville/rp-hal/commit/dab619d6273597fcd9770dcd618987b247f3fc75))
    - Use local rp2040-hal version when building in-crate ([`8690d93`](https://github.com/winksaville/rp-hal/commit/8690d93a6a9f321b90f87be6fa352d2fe8c0fde5))
    - Update WS2812 usage after PIO api's breaking change. ([`c8609e9`](https://github.com/winksaville/rp-hal/commit/c8609e9ef146db7d2db83dd5e16f4772bc90762b))
    - Implement QT Py BSP with example ([`800f71a`](https://github.com/winksaville/rp-hal/commit/800f71a1b8698e396d29ff1a692f3c17358aa15a))
    - Merge pull request #143 from mgottschlag/pio-rework ([`ede25a4`](https://github.com/winksaville/rp-hal/commit/ede25a4f156ac49c8df0e27c3e2347f37e48448e))
    - Add an example using the Feather RP2040's onboard NeoPixel ([`82dfd8e`](https://github.com/winksaville/rp-hal/commit/82dfd8e2cc79683693d6706906ac8c30f5fa330a))
    - Fix clippy warnings and examples in doc comments. ([`4db944a`](https://github.com/winksaville/rp-hal/commit/4db944ad4e1096202f673cd85ddd3e6bcfa0f662))
    - Implements interrupts for GPIO pins. ([`dbd4c7d`](https://github.com/winksaville/rp-hal/commit/dbd4c7dfeac3ddda8cf4742b1b34018deb6dd359))
    - Add changelog entry about PIO changes.. ([`d1bbcea`](https://github.com/winksaville/rp-hal/commit/d1bbceaab4e81ef0a1f12aa9623e827d37eaa286))
    - Rename read_rx/write_tx to read/write. ([`2fc42e0`](https://github.com/winksaville/rp-hal/commit/2fc42e07f235e42cb589bfb72c492013e5e54206))
    - Split RX and TX FIFO functions into different types. ([`207f5ae`](https://github.com/winksaville/rp-hal/commit/207f5aebdbca7fe77823281cd5d8ac01f8f9badf))
    - Identify state machines via generic parameters. ([`dbe7f48`](https://github.com/winksaville/rp-hal/commit/dbe7f48699a0fcc34217f64ffbbb20395ff363d8))
    - Fix bugs spotted in the review. ([`64fa844`](https://github.com/winksaville/rp-hal/commit/64fa8441d8f2db125939c8bdce05973a0756042c))
    - Improve documentation and add an example that uses pio_proc::pio!(). ([`684f483`](https://github.com/winksaville/rp-hal/commit/684f4838590bb5ff809ded117f34364d7c65588e))
    - Differentiate between uninitialized/stopped/running state machines. ([`515eac5`](https://github.com/winksaville/rp-hal/commit/515eac5553e8a06908a73a37e24ec576b26969f5))
    - Enable code sharing between SMs via objects for installed programs. ([`4d97d9f`](https://github.com/winksaville/rp-hal/commit/4d97d9fe75e6627d60ef8855832e4713bbae4c61))
    - Fix marking used instruction space. ([`959f714`](https://github.com/winksaville/rp-hal/commit/959f714fb95b8c585e5d5b539b820d0291178c5e))
    - Fix some doc comments. ([`2ff9ae1`](https://github.com/winksaville/rp-hal/commit/2ff9ae156fcd437a3f087917ee699ec8de8646db))
    - Split PIO into multiple objects that can be moved around separately. ([`e5a7c32`](https://github.com/winksaville/rp-hal/commit/e5a7c325b0ddd38116dbf30d5d921db42f4ac6b5))
    - Merge pull request #137 from 42-technology-ltd/ensure-hal-examples-non-board-specific ([`da89888`](https://github.com/winksaville/rp-hal/commit/da89888ccb5532a66a86e76463db4a556d5d1498))
    - Micontroller ([`49ad970`](https://github.com/winksaville/rp-hal/commit/49ad970d31c6d711f80dfe8cddf9688ed9b0a277))
    - Addressing review comments. ([`fc0075a`](https://github.com/winksaville/rp-hal/commit/fc0075a381c3bf1aaa6623929dcb9d45c56bd72a))
    - Ugh. Thanks, rustfmt. ([`0beedde`](https://github.com/winksaville/rp-hal/commit/0beedde69bbb6b52d719697464615cd4c254661b))
    - Make trait comments more consistent. ([`d251627`](https://github.com/winksaville/rp-hal/commit/d251627e4784448414d111980e198f58ccc5a5fe))
    - Ah, rustfmt. ([`8876159`](https://github.com/winksaville/rp-hal/commit/887615968797886a681a5ca7774e32a9b412a734))
    - Polish the watchdog example. ([`c04f439`](https://github.com/winksaville/rp-hal/commit/c04f439020b2c806bcc4f826b924ff44c3cc5541))
    - Oh, make sure uart example actually builds. ([`b005128`](https://github.com/winksaville/rp-hal/commit/b005128a731801715dd56ae273c5bdd0cd031701))
    - Polish the UART example. ([`7e03772`](https://github.com/winksaville/rp-hal/commit/7e037726878a8d76e4c15c5b66d40bc9eee99546))
    - Cleaning up. ([`b894ab9`](https://github.com/winksaville/rp-hal/commit/b894ab9ce75533574588d463d303e5441d9307b1))
    - Use peripheral clock to describe the clock signal given to peripherals. ([`225eabb`](https://github.com/winksaville/rp-hal/commit/225eabb449815cdb7f9b88f2839e93af8c87a5b2))
    - Say nothing about the default input clock frequency - it's given! ([`c531eb9`](https://github.com/winksaville/rp-hal/commit/c531eb976e128c7f454c6c769908f4223d1790f2))
    - Polish PWM blink example. ([`17afa25`](https://github.com/winksaville/rp-hal/commit/17afa25d2a018953a399ab0d0e4ee1f12ebc8ee5))
    - Polish SPI example. ([`b370bb5`](https://github.com/winksaville/rp-hal/commit/b370bb52702b205e7728418b47e5910132f53cd2))
    - Update LCD example. ([`0336458`](https://github.com/winksaville/rp-hal/commit/03364583448b40eb66214a238393a9c5ffe0de22))
    - Ensure the bootloader static gets documented. ([`29dd755`](https://github.com/winksaville/rp-hal/commit/29dd755b30201bb6802751ce0300c91066daa6d1))
    - Polish I2C example. ([`b7acc7c`](https://github.com/winksaville/rp-hal/commit/b7acc7c3731b5fc3f956873ebe3f7d3974b18b67))
    - Polish GPIO example. ([`193972b`](https://github.com/winksaville/rp-hal/commit/193972bb9fa6ae962e49c24be681a65a01a0cd7f))
    - Remove hard coded clock speed from blink example. ([`d5a07bc`](https://github.com/winksaville/rp-hal/commit/d5a07bc398046abc99ed314eb0ddce9450e3ec2d))
    - Remove hard coded clock speed from ADC example. ([`07c183a`](https://github.com/winksaville/rp-hal/commit/07c183a63650982a86a1bbfdf1383d682630e186))
    - Add picotool to README ([`b3b0c0c`](https://github.com/winksaville/rp-hal/commit/b3b0c0c63abd4bce60243f707b941416f880a474))
    - Link to pio-rs ([`02ea5a4`](https://github.com/winksaville/rp-hal/commit/02ea5a4ac85fa6e1b6968748fd248cf582580543))
    - Expand on page title a little bit ([`6d01432`](https://github.com/winksaville/rp-hal/commit/6d014328ed3da1d733560163a73f8e1743c98e41))
    - Merge pull request #133 from jannic/pio-blinky-example ([`77787e7`](https://github.com/winksaville/rp-hal/commit/77787e760d08a33b558879b239cd28e65c2e369d))
    - Update blinky example. ([`b0bcbe6`](https://github.com/winksaville/rp-hal/commit/b0bcbe68d8e0156c5cf24b40a97d185cfa573516))
    - Update ADC example. ([`ed27dc9`](https://github.com/winksaville/rp-hal/commit/ed27dc9949c8a2faaad29443a83769e214720ea8))
    - README updates. ([`0fa6bf9`](https://github.com/winksaville/rp-hal/commit/0fa6bf9e0e12ac9fee0899b711ee68bc5ad92527))
    - Update comment on top of pio_blink.rs ([`fbe2a88`](https://github.com/winksaville/rp-hal/commit/fbe2a8834f4618fa9f9eeb39f8be0ccb0b4d887d))
    - Update comments in examples/pio_blink.rs ([`c93ea0b`](https://github.com/winksaville/rp-hal/commit/c93ea0b97cc2838cceee61c850b95ec339eccf76))
    - Add a simple example for PIO. ([`b79f859`](https://github.com/winksaville/rp-hal/commit/b79f859d721ed8ec3c7ce88a3a80479600c1c1b7))
    - Fix pico_usb_twitchy_mouse with usbd-hid >= 0.5.1 ([`389e0ea`](https://github.com/winksaville/rp-hal/commit/389e0ea715e751ffd4ccfcce5b716b3400ba389f))
    - Fixed a formatting typo ([`87b29bf`](https://github.com/winksaville/rp-hal/commit/87b29bf9f4b02cd431f30a89f74b069d8d99fcee))
    - Merge pull request #128 from 42-technology-ltd/update-pico-examples ([`58242bc`](https://github.com/winksaville/rp-hal/commit/58242bcc001eec24a4c6aa6b439ed80ab196fb18))
    - Fix the pico lipo example. ([`cbff22b`](https://github.com/winksaville/rp-hal/commit/cbff22b911b7401dc66436d677abaa7e9f6dc140))
    - Correct typo. ([`1e6d14a`](https://github.com/winksaville/rp-hal/commit/1e6d14abb03ca27b45bc9916badcea60822363c4))
    - Add Feather RP2040 README ([`43a22e6`](https://github.com/winksaville/rp-hal/commit/43a22e6e427a8803be0a83ff389e4c7cf27376da))
    - Add Adafruit Macropad README ([`34687a2`](https://github.com/winksaville/rp-hal/commit/34687a2ebe9aba39092ed59a60b3739ddeb19a93))
    - Add Pico Explorer README ([`efe32e6`](https://github.com/winksaville/rp-hal/commit/efe32e627f03488c5b2eb5c34ca4b7b2edff5933))
    - Add Pimoroni Pico Lipo README and example. ([`bc68ee3`](https://github.com/winksaville/rp-hal/commit/bc68ee32fb8be4fa6f703f529ccf4c08e3bcb7ed))
    - Typo in comments. ([`f0fc4ed`](https://github.com/winksaville/rp-hal/commit/f0fc4ed3ad9bb53e1f354d435cda305f4c247d3b))
    - Good ol' clippy. ([`25d87b8`](https://github.com/winksaville/rp-hal/commit/25d87b838b9a78875467ce9f250cc341b7c8bec3))
    - Polishing the USB interrupt examples. ([`b89e728`](https://github.com/winksaville/rp-hal/commit/b89e728e9c5268aedd5e16f52617bfff85e0b3ce))
    - Update non-IRQ USB example. ([`ba6c409`](https://github.com/winksaville/rp-hal/commit/ba6c409f21b862b8163471caaf060552df9c2a6e))
    - Polishing the PWM and USB examples. ([`35f001f`](https://github.com/winksaville/rp-hal/commit/35f001f61decd6ecfa560f83dd2d1fdf18f1bfbf))
    - Polishing the blinky examples. ([`3e036cf`](https://github.com/winksaville/rp-hal/commit/3e036cf9b0174379fabd2b42bfb89d9e60b1aa6b))
    - Merge pull request #126 from 42-technology-ltd/update_pico_docs ([`dc42c71`](https://github.com/winksaville/rp-hal/commit/dc42c714e1a84695e6f9beba788687989afa017d))
    - Mouse twitches the other way. ([`8d4407d`](https://github.com/winksaville/rp-hal/commit/8d4407d846987b913a92dc555bb1876a168c81be))
    - Merge pull request #125 from 42-technology-ltd/add_sparkfun_to_readme ([`1dff385`](https://github.com/winksaville/rp-hal/commit/1dff38551ecd6c787995799d6f87eb87b99aa4bb))
    - Add more example details. ([`410d951`](https://github.com/winksaville/rp-hal/commit/410d95142991c6e0d8af0eeb2adc7a5bd2241ebd))
    - Examples do need to include the board name. ([`0525b3d`](https://github.com/winksaville/rp-hal/commit/0525b3deaf1be6c1dd623eb1f83448101174fe76))
    - WIP README for Pico ([`da89317`](https://github.com/winksaville/rp-hal/commit/da8931721917811565de96751d28483faea001a6))
    - Add README to Pro Micro RP2040 BSP. ([`c992fc9`](https://github.com/winksaville/rp-hal/commit/c992fc9967f3e26ed68c06986dbaddc768a87aa8))
    - Work around enumeration issues with small ep0 max packet size. ([`1d5dd15`](https://github.com/winksaville/rp-hal/commit/1d5dd15092569384d306989a44115ff0351ff52e))
    - Add Pro Micro rainbow example (uses PIO & Timer's Countdown) ([`63dd0b3`](https://github.com/winksaville/rp-hal/commit/63dd0b3066b9d56c1f3de34515f78fe02af7f6d9))
    - Use pio instruction encoding apis ([`833b698`](https://github.com/winksaville/rp-hal/commit/833b69819e0d91b708c1890c25d0f7ecab0964a1))
    - Add port of usb-twitchy-mouse ([`8b1c9fc`](https://github.com/winksaville/rp-hal/commit/8b1c9fc3e5d5f7160550661e7b0f0e21b49a7d35))
    - Add interrupt-driven USB example ([`0cc4614`](https://github.com/winksaville/rp-hal/commit/0cc461488899f71b5d98faf10cfac040a3c30416))
    - Fix adc giving wrong values on sequential reads of multiple channels ([`0e5d582`](https://github.com/winksaville/rp-hal/commit/0e5d582363ae7d7f335269708f729064f40d199c))
    - Update and move readmes ([`216aad2`](https://github.com/winksaville/rp-hal/commit/216aad2c768ae69370a172c246d0d098de559bc5))
    - Merge pull request #96 from 9names/gpio-doc ([`db72171`](https://github.com/winksaville/rp-hal/commit/db7217192a890de7a57e9e257e9aaeba534f0f43))
    - Add doc-example to gpio ([`4c38af0`](https://github.com/winksaville/rp-hal/commit/4c38af00790e7d78ac39d6ad9eba0eca3ee6e8a1))
    - Merge pull request #90 from 9names/i2c-hacks ([`ee5e6ee`](https://github.com/winksaville/rp-hal/commit/ee5e6ee1cb794bac9e3cd910acf0f725f02b3545))
    - Remove setting fields set by default() ([`151b754`](https://github.com/winksaville/rp-hal/commit/151b754d90fc505cc4588a5a47a65eacd44db79f))
    - Switch the modify where C SDK does ([`021221e`](https://github.com/winksaville/rp-hal/commit/021221ede3057ca8fc456fb366369d4587dfb2de))
    - Ensure only pull-up or pull-down is enabled ([`31b9aa8`](https://github.com/winksaville/rp-hal/commit/31b9aa85d1ddba6f67c635bb03dd8aa863996fe0))
    - Enable internal pullups for i2c ([`e00a432`](https://github.com/winksaville/rp-hal/commit/e00a432ed5c792bdf85849236f623145f3d0cf9a))
    - Fix limits on acceptable ranges ([`dbcaf19`](https://github.com/winksaville/rp-hal/commit/dbcaf1933abeee0356a67687741b2866a20e7d4a))
    - Fix transposed variable names ([`50dbb8a`](https://github.com/winksaville/rp-hal/commit/50dbb8a22f74cfd79387bc5d2bc95246e25e3493))
    - Pin pico_explorer to older boot2 ([`6d913f1`](https://github.com/winksaville/rp-hal/commit/6d913f123194f64050362af276ffe9bed1118425))
    - Update CHANGELOG.md ([`5a4d151`](https://github.com/winksaville/rp-hal/commit/5a4d151519325cdc4b9dac851fe0051c328da23a))
    - Implement timer counter ([`04424fb`](https://github.com/winksaville/rp-hal/commit/04424fb7d410c51a2fe74c15af7383c6fad5be48))
    - Prepare for first release ([`d4ec87b`](https://github.com/winksaville/rp-hal/commit/d4ec87b2f7950db71a47155beb224cbbc6968eb3))
    - Correct clobbering registers in pwm subsystem ([`bfe6903`](https://github.com/winksaville/rp-hal/commit/bfe690375193742c74ea80b5c4de9b5d266ae041))
    - Simplify uf2 flashing ([`9d539b0`](https://github.com/winksaville/rp-hal/commit/9d539b0e7d51d08463e2bf18b1a1f92621e05fea))
    - Fix unsigned hardware divide/modulo ([`2d10869`](https://github.com/winksaville/rp-hal/commit/2d1086915c3c178985445edaf559dbbbe8f4b8d3))
    - Pico explorer board support ([`ae8fe51`](https://github.com/winksaville/rp-hal/commit/ae8fe512bda1da8158485a4ccf53b6957001c4b3))
    - Update embedded time ([`bcfbd72`](https://github.com/winksaville/rp-hal/commit/bcfbd72ed116d99610e61cde34f02450c2e8f17d))
    - Also clippy check examples ([`4970075`](https://github.com/winksaville/rp-hal/commit/4970075974f607979f7764e4e1309a256d7ad005))
    - Add Adafruit Macropad BSP ([`25cf81f`](https://github.com/winksaville/rp-hal/commit/25cf81fdfea5276896eab5d60bad1d65e2120379))
    - Warn missing docs, deny in ci ([`148cc2b`](https://github.com/winksaville/rp-hal/commit/148cc2b8ea83cfb035ff6abd76dbe43e6b7c1bc8))
    - Deny warnings in ci ([`1bf47df`](https://github.com/winksaville/rp-hal/commit/1bf47df553e9f048e8e505cbf8e0b40d5ad4b983))
    - Run pwm.rs and pwm_blink.rs through cargo-fmt ([`d2aa2b2`](https://github.com/winksaville/rp-hal/commit/d2aa2b238df58fc34097fd16ccf78fb21a87d1f3))
    - Add bsp for Pico and Pimoroni Pico LiPo ([`c4f30a8`](https://github.com/winksaville/rp-hal/commit/c4f30a8ba6695815f44aaf01312ba84e582b8f93))
    - Add Pico Explorer board support ([`0d4b0e5`](https://github.com/winksaville/rp-hal/commit/0d4b0e564540b723dff41f463d65d0c536bd1842))
    - Fix minor issues ([`711c023`](https://github.com/winksaville/rp-hal/commit/711c0230b1923492bc9bd8c9614a41e92d2070cc))
    - Massive GPIO refactor ([`e3be4f8`](https://github.com/winksaville/rp-hal/commit/e3be4f8025f3fa9344910aa627891ad7bde86980))
    - Split rom_data into safe and unsafe functions ([`71a7057`](https://github.com/winksaville/rp-hal/commit/71a7057b76d9da5bb3bae4520dd9d145430b8429))
    - Add missing clocks ([`e7c2ef3`](https://github.com/winksaville/rp-hal/commit/e7c2ef39c4ff6236e3ebf89c5156e8b143c0e571))
    - Fix gpio docs ([`6edfc60`](https://github.com/winksaville/rp-hal/commit/6edfc609600d23b82d54ab9dfcfef13cb1079130))
    - Fix clippy, run fmt ([`90a6f84`](https://github.com/winksaville/rp-hal/commit/90a6f8414daaca9ab1e31029b5252b097dc67733))
    - Change all write to modify ([`0d19834`](https://github.com/winksaville/rp-hal/commit/0d19834b2ede6deb3f8c34ddb77ce02702325f11))
    - Cargo fmt ([`4220b45`](https://github.com/winksaville/rp-hal/commit/4220b45c24f0b57faeec41fe5976a15a96a6ffd4))
    - Initial commit on clocks ([`ef7f8fe`](https://github.com/winksaville/rp-hal/commit/ef7f8fe9b7844364e1f59f048cce52f791434225))
    - Add documentation to public functions and struct, fix logic issue with max period ([`c4cd2ff`](https://github.com/winksaville/rp-hal/commit/c4cd2ffe52a4844dd43a81594df3b0e9bcdfddc3))
    - Panic if period exceeds maximum value, fmt ([`c568f0d`](https://github.com/winksaville/rp-hal/commit/c568f0d3df08e7f5e4b6280f066a0e7b446774d2))
    - Add pause_on_debug, disable watchdog prior to enabling ([`cdd9a55`](https://github.com/winksaville/rp-hal/commit/cdd9a553ad610fbe0fed10e53be992871355bcff))
    - Fix logic issue with delay_ms ([`fe72637`](https://github.com/winksaville/rp-hal/commit/fe72637972895c16f07813349297943264531f5a))
    - Initial watchdog implementation ([`596bea3`](https://github.com/winksaville/rp-hal/commit/596bea309b89e5104c512ff93474d41a5f8219ee))
    - Merge pull request #38 from anall/bugfix/pll-uart-reset ([`9bef082`](https://github.com/winksaville/rp-hal/commit/9bef0821d9217898295fe794cff180e75f01c6f4))
    - Add `SubsystemReset` trait to handle subsystem resets ([`8d0fde2`](https://github.com/winksaville/rp-hal/commit/8d0fde20c69bf00ca5f75fab6aef83113f757b43))
    - Merge pull request #36 from anall/feature/sio ([`9e7e785`](https://github.com/winksaville/rp-hal/commit/9e7e785e22efa4f106369b1249c53e314b49c4b6))
    - Typo fix, rustfmt ([`35464a1`](https://github.com/winksaville/rp-hal/commit/35464a1c4b2c35d6a8e9b26c0ac529a3260bacb7))
    - Add module to manage ownership of parts of SIO ([`2ef1343`](https://github.com/winksaville/rp-hal/commit/2ef1343c053d2aefa53dfc5c67a67b159a9405c2))
    - Merge pull request #28 from Nic0w/uart ([`877c967`](https://github.com/winksaville/rp-hal/commit/877c967466d865d5371578d4ae3b665bc36849c8))
    - Merge pull request #27 from Nic0w/pll ([`c5da765`](https://github.com/winksaville/rp-hal/commit/c5da7659c9469637751764e7f4b51587255c0ea5))
    - Clippy, second pass for errors in CI. ([`9b082b0`](https://github.com/winksaville/rp-hal/commit/9b082b012d98bc6de4577f461eeb8fb33f04a9b0))
    - Clippy, second pass for errors in CI. ([`a663b1f`](https://github.com/winksaville/rp-hal/commit/a663b1f55295d215fd27344402f31ef809104824))
    - Merge branch 'uart' of github.com:Nic0w/rp-hal into uart ([`e18111d`](https://github.com/winksaville/rp-hal/commit/e18111d5645cc544278d97f9216fd041879465b3))
    - Cargo clippy & fmt ([`020c9d9`](https://github.com/winksaville/rp-hal/commit/020c9d9a3de9057ee2b79be40e00e24bcec4101d))
    - Change comment on baudrate calculation ([`c35358f`](https://github.com/winksaville/rp-hal/commit/c35358f475ea02428952079f6ad901cdd048d928))
    - Satisfies clippy ([`64dee52`](https://github.com/winksaville/rp-hal/commit/64dee52dd57cfe4f206b50d4160547c58360d881))
    - Remove duplicate entry in Cargo.toml ([`72127aa`](https://github.com/winksaville/rp-hal/commit/72127aa8e7b41e50f06e5a71c4ff2395fddd79ff))
    - Merge branch 'main' into uart ([`31b0230`](https://github.com/winksaville/rp-hal/commit/31b0230da193562bd8c948672544f20c7ebb20a9))
    - Merge pull request #24 from Nitori-/basic-gpio ([`19cb392`](https://github.com/winksaville/rp-hal/commit/19cb392205f7cedbfb42c4eb42670b24c701affd))
    - Merge branch 'main' into basic-gpio ([`d26e13c`](https://github.com/winksaville/rp-hal/commit/d26e13c5ef88aa5fa4982cb639cb48515d46ff87))
    - Merge pull request #32 from 9names/ci_improvement ([`e30d4af`](https://github.com/winksaville/rp-hal/commit/e30d4af814cd823b8aa1fd2e7b10936ea65b682f))
    - Better comments and renamed variable names for more clarity. ([`8586f98`](https://github.com/winksaville/rp-hal/commit/8586f98c02bfe95893dc534f87d789f9ca2a9840))
    - Consistency re. clear_bit/set_bit. ([`be78a5c`](https://github.com/winksaville/rp-hal/commit/be78a5c792bb5c073aa7966a51ebb155461eeb90))
    - Pulling the integer out of the frequency first. ([`ac2af75`](https://github.com/winksaville/rp-hal/commit/ac2af7582ee4503d7db4b96996bfa1b16cc99919))
    - Fix comments on {read,write}_raw() functions ([`d9b1b2b`](https://github.com/winksaville/rp-hal/commit/d9b1b2b1ec77d8a26fb351be6add2cd981d362c3))
    - Add #Safety tag to unsafe rationale docstring ([`416baf6`](https://github.com/winksaville/rp-hal/commit/416baf64054ed038af804408ca03a8d861a4db9b))
    - Move tests into seperate workflow ([`691f43c`](https://github.com/winksaville/rp-hal/commit/691f43c17baee0a2d45cc4861f66629996bd8a1f))
    - Move clippy into seperate workflow ([`41c6db6`](https://github.com/winksaville/rp-hal/commit/41c6db68114933202b4111348b133bf7f8130d57))
    - Move rustfmt to seperateworkflow ([`95a1080`](https://github.com/winksaville/rp-hal/commit/95a1080a4615be5e33ad544d579c54e2addd1269))
    - Merge branch 'main' into basic-gpio ([`7588f76`](https://github.com/winksaville/rp-hal/commit/7588f7684408fec88451b33029cc9f44a78f2778))
    - Propagate read errors. ([`8d29464`](https://github.com/winksaville/rp-hal/commit/8d29464ee309e8875df04fe48372e466e0c30c12))
    - Cargo fmt ([`992bcdf`](https://github.com/winksaville/rp-hal/commit/992bcdf47b576f538e407da327f9f7d5c51c84cd))
    - Move serial traits impl. back to uart.rs ([`abf91a3`](https://github.com/winksaville/rp-hal/commit/abf91a36873f61e2faa44fa85962de23952ea18f))
    - Read errors. ([`835ad7a`](https://github.com/winksaville/rp-hal/commit/835ad7a5c1e55b9ef850c5ac411246e45289f567))
    - Move checks in new() so initialize() cannot fail. ([`5620bdb`](https://github.com/winksaville/rp-hal/commit/5620bdbd07e4e7fdb343700ead6573afc77c73b5))
    - Cargo fmt pass. ([`eb4ebc7`](https://github.com/winksaville/rp-hal/commit/eb4ebc782a9d9d70b4e7f5f2e7c582ff2466dc5f))
    - Merge branch 'pll' of github.com:Nic0w/rp-hal into pll ([`e91e124`](https://github.com/winksaville/rp-hal/commit/e91e12448458d3f987c1ba48d0db08e548841539))
    - Using modify() to clear specific bits instead of a blanket 0 on all bits. ([`eb376cf`](https://github.com/winksaville/rp-hal/commit/eb376cf47b4ad485394f433dd2452e2b93db11ee))
    - Fix typo on post_div check ([`5726bef`](https://github.com/winksaville/rp-hal/commit/5726bef879d776e84c7bf070a2e602215e22c8fb))
    - Fix type conversion issue ([`20c35d5`](https://github.com/winksaville/rp-hal/commit/20c35d5e14a6a14bcb763d5bf5c373729b4ea2bc))
    - Move PLL parameters into a struct to help testability and reconfiguration of the PLL. ([`6499981`](https://github.com/winksaville/rp-hal/commit/649998189f5e3de4fa9f27cdda723c72b4081998))
    - Working implementation of a PLL HAL. ([`9be7c41`](https://github.com/winksaville/rp-hal/commit/9be7c41400eb71a1335d9a4b814fbb6f339ef36c))
    - Merge pull request #30 from 9names/fix_xosc_warning ([`48dd806`](https://github.com/winksaville/rp-hal/commit/48dd8069b867a3c12cc83499707a47d6273f2b6d))
    - Remove redundant field name ([`010a5ca`](https://github.com/winksaville/rp-hal/commit/010a5cabf3b6967489bda8a24759dbd425e4d6f4))
    - Autoformatted using cargo fmt ([`f21648d`](https://github.com/winksaville/rp-hal/commit/f21648de933e24a330cdb05759590e5db442ba74))
    - Remove unneeded unsafe ([`1b42913`](https://github.com/winksaville/rp-hal/commit/1b4291307758b71dbdfb4ba28ec300154d169aa1))
    - Merge pull request #29 from tdittr/feature/doc-tests-in-ci ([`3bdc338`](https://github.com/winksaville/rp-hal/commit/3bdc338a0d7c852cb06bf130a6c30b0968f7cd77))
    - Merge pull request #25 from Nic0w/xosc ([`f728de5`](https://github.com/winksaville/rp-hal/commit/f728de5efbdb7a021a35006bb7e55828f75001a6))
    - Add `cargo test` to CI run and fix an error found by it ([`39f02c4`](https://github.com/winksaville/rp-hal/commit/39f02c4a441dad79f6e8bbb3199130a3f1d61c1a))
    - Implement embedded_hal::serial traits for the UART. ([`f3fba80`](https://github.com/winksaville/rp-hal/commit/f3fba80a713b632bee7190db8105065864518028))
    - Error needs to derive Debug if we want to unwrap. ([`50a428e`](https://github.com/winksaville/rp-hal/commit/50a428e2ad1262eefdfe02feb2bae0854d22616c))
    - Fix ARM toolchain apt package name ([`a4b15a3`](https://github.com/winksaville/rp-hal/commit/a4b15a3547522bcac10a9c54eae2bd9390d9991b))
    - Apt-get requires sudo ([`09d9247`](https://github.com/winksaville/rp-hal/commit/09d9247f2f076a14b775b1cce9a695401241c07c))
    - Install arm-none-eabi-gcc in CI ([`0badff4`](https://github.com/winksaville/rp-hal/commit/0badff4f1cdb6f1e2d476f288f3a25da2966e332))
    - Also check examples ([`d738626`](https://github.com/winksaville/rp-hal/commit/d738626f70cfe40ef2659d262887af12578520df))
    - Merge branch 'main' of github.com:rp-rs/rp-hal into basic-gpio ([`0ff5152`](https://github.com/winksaville/rp-hal/commit/0ff51520f54b0472ee508ff968e41e9d4dee8cb7))
    - Merge pull request #23 from Nitori-/ci ([`ca8273b`](https://github.com/winksaville/rp-hal/commit/ca8273b2c58aedebd662be7b4f7ecfa96c0bd4ff))
    - Merge branch 'uart' of github.com:Nic0w/rp-hal into uart ([`920d0dc`](https://github.com/winksaville/rp-hal/commit/920d0dc897b35eaf8ba4c77f95c5f98847d9cc59))
    - Multiple changes addressing @tdittr 's comments. ([`4d949f7`](https://github.com/winksaville/rp-hal/commit/4d949f7310cb6f3af1a69b0c182fcdc0b41dbad6))
    - Disable the UART for real when disabling UART. ([`aa3fe8f`](https://github.com/winksaville/rp-hal/commit/aa3fe8fd2023e02a7c7ea22ea43533a49ccf23dc))
    - Cosmetics. ([`c50a5b6`](https://github.com/winksaville/rp-hal/commit/c50a5b60014292ab8d4d5dc0bf318d363dd4a08a))
    - Increment byte_written after write has happened. ([`f9254fd`](https://github.com/winksaville/rp-hal/commit/f9254fdffa29fc62ad1a576f58669ea532536dc2))
    - Fix typo on post_div check ([`2462c43`](https://github.com/winksaville/rp-hal/commit/2462c430b98fb77d33bb93b7031db77629300a6e))
    - Fix type conversion issue ([`c3bc1bb`](https://github.com/winksaville/rp-hal/commit/c3bc1bbaf87791e7910a296e28e92eae24900267))
    - Pin ubuntu version ([`e9721e1`](https://github.com/winksaville/rp-hal/commit/e9721e14c252f3f7adb9abb8969bffb48a938fa1))
    - Update rp2040-hal/src/gpio.rs ([`c4ae152`](https://github.com/winksaville/rp-hal/commit/c4ae152fda7a5499e1e4bf8cf4fb2f55d57e69f5))
    - Concentrate the unsafe register constructs ([`eaea9ae`](https://github.com/winksaville/rp-hal/commit/eaea9ae1ed663907ed434bc098cc35798023a654))
    - Pull pads out of reset and wait ([`8290368`](https://github.com/winksaville/rp-hal/commit/8290368c10a9ca54bd0ea5b5ffb8c63ce213371f))
    - Do reset in a good way instead of a wacky way ([`7e45c96`](https://github.com/winksaville/rp-hal/commit/7e45c96a658be5c2c4287503e7a68d92e3eae65a))
    - More review comments ([`b3b7677`](https://github.com/winksaville/rp-hal/commit/b3b7677f82fd59b1f1da1f94816a036a1750cb81))
    - Move PLL parameters into a struct to help testability and reconfiguration of the PLL. ([`6157ce5`](https://github.com/winksaville/rp-hal/commit/6157ce552fbfdfa1403920fadb345448299c451d))
    - Apply suggestions from code review ([`037fc66`](https://github.com/winksaville/rp-hal/commit/037fc665b2ce57a43a070258ac529b0ee59ed811))
    - Adding blocking helper method to setup the XOSC easily. ([`2a704a7`](https://github.com/winksaville/rp-hal/commit/2a704a73f0fa0178e0775c2aec64183061deee4c))
    - Working implementation of an UART HAL. ([`b9080d0`](https://github.com/winksaville/rp-hal/commit/b9080d0a926891295922700590d3d5f673969472))
    - Working implementation of a PLL HAL. ([`ff418b0`](https://github.com/winksaville/rp-hal/commit/ff418b04531799dc36ad943c5700b1eaacc59050))
    - Ignores Cargo.lock and target/*. ([`b0de7c9`](https://github.com/winksaville/rp-hal/commit/b0de7c9be6fba15be20aba092436464c26a61f96))
    - Fix compilation issues. ([`8f6aea6`](https://github.com/winksaville/rp-hal/commit/8f6aea6a31b04b43851b4755cd463b3e11d84b97))
    - Fix frequency range check. ([`72694a0`](https://github.com/winksaville/rp-hal/commit/72694a07b5bff9dd0531e4042c08c5fb04e6824c))
    - Apply suggestions from code review ([`cb51448`](https://github.com/winksaville/rp-hal/commit/cb51448089620fa69c4333a634bc2f331ff5ea41))
    - Also build all examples ([`cc1a1be`](https://github.com/winksaville/rp-hal/commit/cc1a1bee2cc0d5dd978004b81988bf6355527823))
    - Add documentation ([`422a45f`](https://github.com/winksaville/rp-hal/commit/422a45fbc5b6779163912c7f88aca8d8645d2172))
    - Finish configuration options for IOs ([`94f67f7`](https://github.com/winksaville/rp-hal/commit/94f67f7ecac49c3b3e00c5b0e5ed259cd6ae2903))
    - Fixing calculation bug pointed out by @tdittr ([`d5cbd44`](https://github.com/winksaville/rp-hal/commit/d5cbd44adeb9137df7394b7daf887aafe5f2703c))
    - Block input reads on Unknown state ([`3536604`](https://github.com/winksaville/rp-hal/commit/3536604b9e5b83056480f21d05da032a49220f73))
    - Multiple changes related to @tdittr 's comments ([`568cafe`](https://github.com/winksaville/rp-hal/commit/568cafe2d109ac3263c530b5adad708cf6efc063))
    - Cleanup wacky imports in examples ([`2e5c1fc`](https://github.com/winksaville/rp-hal/commit/2e5c1fc0e36e812dd05ca21614dd5f9b09191f38))
    - Add input support, examples, SIO/PADS ownership ([`2c3a095`](https://github.com/winksaville/rp-hal/commit/2c3a0956fa321062c0a7b68ad716596ce550ed1c))
    - Remove line as it builds fine without it. ([`ed1e847`](https://github.com/winksaville/rp-hal/commit/ed1e847618cccc54780963e664ffb1ef043319e3))
    - Pass --all to cargo check ([`5dfa550`](https://github.com/winksaville/rp-hal/commit/5dfa550663788399d5c1be1235f326e2a4c89abe))
    - Remove Cargo.lock ([`3c528c6`](https://github.com/winksaville/rp-hal/commit/3c528c6a93b754f211f7d7d3c818b97240bdeb89))
    - Working HAL for the XOSC ([`d0d9291`](https://github.com/winksaville/rp-hal/commit/d0d9291cdee12bcdf9c294cacba94dc6e6da9eb6))
    - Add basic output support for GPIOs ([`45580ec`](https://github.com/winksaville/rp-hal/commit/45580ec4c8c9955ba7cdc403ce3ba30ae6774e9f))
    - Also run the checks on PRs ([`778a87d`](https://github.com/winksaville/rp-hal/commit/778a87dfaaa176857d169924336d0d5147a4a824))
    - Run `cargo fmt` ([`d318d05`](https://github.com/winksaville/rp-hal/commit/d318d050673b1b2113fe11935e8ca82ac99229d7))
    - Add CI checks ([`63607e5`](https://github.com/winksaville/rp-hal/commit/63607e5533ddf2194cb0756673303d49ee19b175))
    - Merge pull request #20 from jannic/fix-rom-functions ([`b96339c`](https://github.com/winksaville/rp-hal/commit/b96339c41754b9834756d139d9077608eef104e8))
    - Rom function git_revision() does return an u32, not a &str ([`5494ce7`](https://github.com/winksaville/rp-hal/commit/5494ce753922b4b996a6d7a664c4dbda1c880652))
    - Fix rom_table_lookup ([`d6231bd`](https://github.com/winksaville/rp-hal/commit/d6231bd3ecde9de064beaf9c3b05e05e6bbabbe0))
    - Merge pull request #16 from rp-rs/rom-functions ([`be7dd11`](https://github.com/winksaville/rp-hal/commit/be7dd1105744fbae9c63f1d05a623775e6114180))
    - Fix type error ([`913c5fb`](https://github.com/winksaville/rp-hal/commit/913c5fb0b239e7097057d28df9b892cf4aa004a9))
    - Make rom_funcs functions call function instead of returning it ([`1848789`](https://github.com/winksaville/rp-hal/commit/1848789ca3118279d636de10006f5cafc8338444))
    - Merge pull request #15 from rp-rs/pi-workspace ([`2972cfe`](https://github.com/winksaville/rp-hal/commit/2972cfebcb9072f83594e52d25c3941a88dd80a1))
    - Add workspaces to project ([`e44d561`](https://github.com/winksaville/rp-hal/commit/e44d561ef2421497fe2eeb2164a5caceea68eb94))
    - Merge pull request #11 from devsnek/rom-stuff ([`1744151`](https://github.com/winksaville/rp-hal/commit/17441510252fb3258e372f3e47d563a04d6102a2))
    - Add comments to rom content ([`a9a8df8`](https://github.com/winksaville/rp-hal/commit/a9a8df8c794c163fbb5e6d4f79f32d1196e01b28))
    - Change `rom_table_lookup` to use the rom's built in one ([`6eccce5`](https://github.com/winksaville/rp-hal/commit/6eccce595c6afb53e1708b9d68a5658d9e076619))
    - Add rom content ([`1c75ed3`](https://github.com/winksaville/rp-hal/commit/1c75ed3844f5c36cb7cb81ab0ef424a333d0fa80))
    - Merge pull request #3 from johnbatty/main ([`5159d04`](https://github.com/winksaville/rp-hal/commit/5159d0409761ad8059a4c86e9a5ba449ee727b8d))
    - Rename CONTRIBUTING.md to CODE_OF_CONDUCT.md ([`8ef2d6f`](https://github.com/winksaville/rp-hal/commit/8ef2d6fbab1536b375e8fd00877e072e503eb78b))
    - Create CONTRIBUTING.md ([`713e749`](https://github.com/winksaville/rp-hal/commit/713e7491b7d337a2b53e231ef4c3a49485389a03))
    - Add .cargo/config defining the build target ([`0d22828`](https://github.com/winksaville/rp-hal/commit/0d228286cbb3cfe78a7f3c184a922a045d477a96))
    - Merge pull request #2 from rp-rs/eolder-skeleton ([`7809177`](https://github.com/winksaville/rp-hal/commit/780917774ec79e7f93b2934bfe724c05921db18f))
    - Added skeleton for HAL and updated readme ([`98baabe`](https://github.com/winksaville/rp-hal/commit/98baabec937532658127b9fe28873e458be1c0cc))
    - Update README.md ([`36b9892`](https://github.com/winksaville/rp-hal/commit/36b9892c43b4db2152c72e570ea2c090b3c44fe3))
    - Update README.md ([`d836b92`](https://github.com/winksaville/rp-hal/commit/d836b9231d0925649cb89715e8d291ebdddb43f0))
    - Update README.md ([`e9e3b39`](https://github.com/winksaville/rp-hal/commit/e9e3b394202103b30f9dacdcfabb6bb6203ba62b))
    - Initial Commit: Updated author information. ([`22a3669`](https://github.com/winksaville/rp-hal/commit/22a3669a9d5cdaa303881f28a4a7e1b2cc845ecf))
</details>

