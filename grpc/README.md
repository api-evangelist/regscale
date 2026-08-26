# RegScale gRPC contracts

Reconstructed from the **first-party** `rs-data` distribution RegScale publishes on PyPI
(`rs-data` 1.5.0, sdist `rs_data-1.5.0.tar.gz`, uploaded 2026-05-05), described by RegScale
as the *"RegScale gRPC contract library — assets, issues, and vulnerabilities"*.

RegScale does not publish the `.proto` files themselves in a public repository
(`github.com/regscale/rs-data` returns 404 / private). The `.proto` files here were rendered
from the compiled `FileDescriptorProto` embedded in RegScale's own generated
`*_pb2.py` modules — i.e. the exact wire contract RegScale shipped, decompiled, not authored.
Original `source:` filenames from the descriptors are preserved below.

| File here | Descriptor `name` | Package |
|---|---|---|
| `regscale-asset.proto` | `regscale/assets/v1/asset.proto` | `regscale.assets.v1` |
| `regscale-asset-service.proto` | `regscale/assets/v1/asset_service.proto` | `regscale.assets.v1` |
| `regscale-issue.proto` | `regscale/issues/v1/issue.proto` | `regscale.issues.v1` |
| `regscale-issue-service.proto` | `regscale/issues/v1/issue_service.proto` | `regscale.issues.v1` |
| `regscale-vuln.proto` | `regscale/vulns/v1/vuln.proto` | `regscale.vulns.v1` |
| `regscale-vuln-service.proto` | `regscale/vulns/v1/vuln_service.proto` | `regscale.vulns.v1` |

Ownership: every descriptor declares the `regscale.*.v1` protobuf package and the
`RegScale.Assets.V1` / `RegScale.Issues.V1` / `RegScale.Vulns.V1` C# namespace, and the
distribution's `pyproject.toml` names RegScale as the author. The contract is RegScale's own.
