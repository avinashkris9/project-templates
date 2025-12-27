# Project Templates

Some copier templates

## Usage

### Prerequisites

```bash
# Install Copier
pip install copier

# Or using pipx (recommended)
pipx install copier
```

### Generate from Template

```bash
# Interactive mode
copier copy gh:YOUR_USERNAME/devops-copier-templates

# Specify subdirectory
copier copy gh:YOUR_USERNAME/devops-copier-templates --subdirectory=bash-script my-script

# With answers
copier copy gh:YOUR_USERNAME/devops-copier-templates \
  --subdirectory=python-cli \
  --data project_name="My CLI Tool" \
  my-cli-tool
```

### Update Existing Project

```bash
cd my-project
copier update
```

## Resources

- [Copier Documentation](https://copier.readthedocs.io/)
