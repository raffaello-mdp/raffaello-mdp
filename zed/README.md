# Zed Configuration

My [Zed](https://zed.dev) editor settings, tuned for platform engineering work: Kubernetes/Helm, OpenTofu/Terraform, Go and shell.

## Install

```bash
cp zed/settings.json ~/.config/zed/settings.json
```

## Highlights

- **Panel layout:** project panel left, everything else (outline, git, agent, collaboration) docked right.
- **Helm detection:** `values*.yaml`, `**/templates/**` and `helmfile.d/**` are mapped to the Helm language so Go templating does not break YAML parsing.
- **OpenTofu:** `.tf` / `.tfvars` mapped to the OpenTofu languages, formatted through `tofu fmt -` for both Terraform and HCL.
- **YAML LSP:** key ordering enforced, single-quote formatting, schema store disabled in favour of explicit schema mappings.
- **gopls:** full inlay hints (parameter names, variable types, composite literals, constant values).
- **Theme:** follows the system appearance, One Light / One Dark.
