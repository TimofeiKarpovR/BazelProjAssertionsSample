# BazelProjAssertionsSample

Problem: Test assertions are not shown in the code

# Steps to reproduce:
- run `bazel run xcodeproj`
- open generated App.xcodeproj
- run `FooTests`

# Result
<img width="800" alt="Screenshot 2024-11-22 at 12 38 33" src="https://github.com/user-attachments/assets/de644200-c1c4-4f90-83f5-1b451735d93f">

# Expected result
<img width="800" alt="Screenshot 2024-11-22 at 12 40 38" src="https://github.com/user-attachments/assets/5aabbc0e-34cd-436f-96cf-7ac04b9a0af4">

Screenshot was made with these changes:

```
bazel_dep(
    name = "rules_swift",
    version = "1.18.0",
    repo_name = "build_bazel_rules_swift",
)
bazel_dep(
    name = "rules_apple",
    version = "3.2.0",
    repo_name = "build_bazel_rules_apple",
)
```
