# c-cpp-github-release

Reusable GitHub Actions workflow for C and C++ library releases.

Repositories provide a script such as `scripts/release-ci.sh` that accepts
`--os`, `--arch`, and `--output`, builds/tests both static and shared variants,
verifies their linkage with platform-native tools, and writes six ZIP files to
the output directory. The shared workflow handles the Windows, macOS, Linux,
x86_64, and arm64 matrix, cancellation, artifact collection, checksums, and
release publication.
