---
title: Install GroupDocs.Search for Python via .NET
linkTitle: "Installation"
second_title: GroupDocs.Search for Python via .NET API References
description: "Install GroupDocs.Search for Python via .NET on Windows, Linux, or macOS - from PyPI or from a pre-downloaded wheel, including Intel and Apple Silicon builds."
type: docs
url: /python-net/guides/installation/
is_root: false
weight: 10
---


GroupDocs.Search for Python via .NET is distributed as a pre-built wheel on [PyPI](https://pypi.org/project/groupdocs-search-net/). The PyPI index hosts a separate wheel for each supported platform, and `pip` picks the correct one automatically. Each wheel is self-contained: it bundles the embedded .NET runtime and every managed dependency, so no Microsoft Office, OpenOffice, or separate runtime install is required.

Before you install, review the [System Requirements](https://docs.groupdocs.com/search/python-net/system-requirements/). The wheels need 64-bit Python 3.5-3.14 and pip 20.3 or newer, and run on Windows, on Linux with glibc 2.27 or newer, and on macOS 13 or newer. On Linux, install ICU and `libgdiplus`; on macOS, install `mono-libgdiplus` (see [Platform Prerequisites](#platform-prerequisites)).

## Install Package from PyPI

Open a terminal and run the install command for your platform:

{{< tabs "install-pypi">}}
{{< tab "Windows" >}}
```ps
py -m pip install groupdocs-search-net
```
{{< /tab >}}
{{< tab "Linux" >}}
```bash
python3 -m pip install groupdocs-search-net
```
{{< /tab >}}
{{< tab "macOS" >}}
```bash
python3 -m pip install groupdocs-search-net
```
{{< /tab >}}
{{< /tabs >}}

After running the command you should see output similar to:

```bash
Collecting groupdocs-search-net
  Downloading groupdocs_search_net-26.10.0-py3-none-win_amd64.whl (255.3 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 255.3/255.3 MB 3.1 MB/s eta 0:00:00
Installing collected packages: groupdocs-search-net
Successfully installed groupdocs-search-net-26.10.0
```

The wheel file name will include a platform suffix that matches your operating system - for example `manylinux_2_27_x86_64` on Linux, `macosx_13_0_arm64` on Apple Silicon, or `win_amd64` on 64-bit Windows.

## Add the Package to `requirements.txt`

For reproducible environments, pin the package version in your `requirements.txt`:

```txt
groupdocs-search-net==26.10.0
```

Then install all dependencies in one step:

```bash
pip install -r requirements.txt
```

## Install from a Pre-Downloaded Wheel

If your build environment cannot reach PyPI, download the appropriate wheel from the [GroupDocs Releases website](https://releases.groupdocs.com/search/python-net/) and install it locally. Wheels are published for the following four platforms:

| Platform | Wheel file name ends with | Oldest system |
| --- | --- | --- |
| Windows 64-bit | `py3-none-win_amd64.whl` | Windows 10, Windows Server 2016 |
| Linux x64 (glibc) | `py3-none-manylinux_2_27_x86_64.whl` | glibc 2.27 (Ubuntu 18.04, Debian 10, RHEL 8) |
| macOS Apple Silicon (M-series) | `py3-none-macosx_13_0_arm64.whl` | macOS 13 |
| macOS Intel | `py3-none-macosx_13_0_x86_64.whl` | macOS 13 |

The file names state the oldest system each wheel runs on, so pip 20.3 or newer refuses a wheel the system cannot run. There is no 32-bit wheel.

Place the downloaded wheel into your project folder, then install it:

{{< tabs "install-wheel">}}
{{< tab "Windows (64-bit)" >}}
```ps
py -m pip install .\groupdocs_search_net-26.10.0-py3-none-win_amd64.whl
```
{{< /tab >}}
{{< tab "Linux (glibc)" >}}
```bash
python3 -m pip install ./groupdocs_search_net-26.10.0-py3-none-manylinux_2_27_x86_64.whl
```
{{< /tab >}}
{{< tab "macOS (Intel)" >}}
```bash
python3 -m pip install ./groupdocs_search_net-26.10.0-py3-none-macosx_13_0_x86_64.whl
```
{{< /tab >}}
{{< tab "macOS (Apple Silicon)" >}}
```bash
python3 -m pip install ./groupdocs_search_net-26.10.0-py3-none-macosx_13_0_arm64.whl
```
{{< /tab >}}
{{< /tabs >}}

Name the wheel file explicitly: PowerShell does not expand a `*` wildcard for a native command, so `pip install groupdocs_search_net-*.whl` fails there.

Expected output (Linux):

```bash
Processing ./groupdocs_search_net-26.10.0-py3-none-manylinux_2_27_x86_64.whl
Installing collected packages: groupdocs-search-net
Successfully installed groupdocs-search-net-26.10.0
```

If pip reports `is not a supported wheel on this platform`, pip is older than 20.3 or the system is older than the wheel needs: run `python -m pip install --upgrade pip` first. Python 3.5 needs pip 20.3.4, the last release for it. On an Intel Mac, a Python built against an old SDK reports macOS 10.16; use pip 24.1 or newer, or `SYSTEM_VERSION_COMPAT=0 pip install ...`.

## Platform Prerequisites

On Windows no extra steps are required. On Linux, install ICU and `libgdiplus`; on macOS, `mono-libgdiplus`. The [System Requirements](https://docs.groupdocs.com/search/python-net/system-requirements/) page explains what each one is for.

{{< tabs "platform-prereqs">}}
{{< tab "Linux" >}}
```bash
sudo apt-get update
sudo apt-get install -y libicu-dev libgdiplus
```
{{< /tab >}}
{{< tab "macOS" >}}
```bash
brew install mono-libgdiplus
```
{{< /tab >}}
{{< /tabs >}}

ICU is required: without it the process aborts at the first call into the engine. `libgdiplus` serves presentations: without it, ODP and PPT files are left out of the index, and the index's `error_occurred` event reports why. No fonts are needed.

## Verify the Installation

Confirm the package imported correctly:

```bash
python -c "import groupdocs.search; print('GroupDocs.Search is ready')"
```

You can also list the installed package with `pip show groupdocs-search-net` to confirm the version and location.

The first call into the engine takes about a second. On Windows, when a license is applied, the first call in a process takes 15-30 seconds: that is the engine's license check, which runs once per process.

## Next Steps

- Follow the [Hello, World!](/search/python-net/guides/hello-world/) guide to index and search your first documents.
- Read the [Features Overview](/search/python-net/guides/features-overview/) to see everything you can do.
- Clone the [examples repository](https://github.com/groupdocs-search/GroupDocs.Search-for-Python-via-.NET) and read [How to Run Examples](https://docs.groupdocs.com/search/python-net/how-to-run-examples/) to try every documented scenario locally.
