# {{ script_name }}

{{ script_description }}


## Features

{% if include_logging %}- Comprehensive logging with configurable log levels{% endif %}
{% if include_arg_parsing %}- Command-line argument parsing{% endif %}
{% if include_error_handling %}- Robust error handling and cleanup{% endif %}
{% if include_help %}- Built-in help and usage documentation{% endif %}
{% if include_colors %}- Colored output for better readability{% endif %}
{% if include_config_file %}- Configuration file support ({{ config_file_format }}){% endif %}
{% if include_dependencies_check %}- Automatic dependency checking{% endif %}

## Requirements

- Bash 4.0 or higher

## Installation

```bash
# Clone or download the script
chmod +x {{ script_kebab_case }}.sh

# Optionally, move to a directory in your PATH
{% if install_to_bin %}sudo cp {{ script_kebab_case }}.sh /usr/local/bin/{{ script_kebab_case }}{% else %}# mv {{ script_kebab_case }}.sh ~/bin/{{ script_kebab_case }}{% endif %}
```

## Usage

```bash
# Basic usage
./{{ script_kebab_case }}.sh

# Show help
./{{ script_kebab_case }}.sh --help

# Verbose output
./{{ script_kebab_case }}.sh --verbose

# Dry run mode
./{{ script_kebab_case }}.sh --dry-run
{% if include_logging %}
# Set log level
./{{ script_kebab_case }}.sh --log-level DEBUG
{% endif %}
```

### Debug Mode

Enable debug output:
```bash
DEBUG=1 ./{{ script_kebab_case }}.sh
```