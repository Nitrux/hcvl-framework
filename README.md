# Hardware Compatibility Validation Layer (HCVL)

A framework that ensures that Nitrux runs in a predictable, supportable, and well-understood environment. It reduces ambiguity by validating four key areas:

- CPU capability validation:
    - HCVL ensures the system runs only on processors that support the required instruction set. If the requirement fails, the system stops early in boot and explains why. Early validation prevents users from running into subtle breakage later.
- GPU and ISO alignment:
    - HCVL verifies that the hardware graphics stack matches the ISO variant (Mesa or NVIDIA). If it detects a mismatch, HCVL informs the user early before the graphical session starts. Early notification avoids confusing failures and improves support clarity.
- Environment and resource awareness:
    - HCVL detects virtualized environments and low-resource systems and clearly communicates compatibility requirements. Clear communication ensures that feedback, diagnostics, and performance impressions reflect the environment Nitrux targets.
- Workflow clarity and system-model consistency:
    - HCVL intercepts unsupported host-level workflows (such as legacy package managers or unmanaged binaries) and explains alternatives. Interception prevents accidental misuse and helps maintain the integrity and reliability of the system.

# Licensing

The license for this repository and its contents is **BSD-3-Clause**.

# Issues
If you find problems with the contents of this repository please create an issue.

©2026 Nitrux Latinoamericana S.C.
