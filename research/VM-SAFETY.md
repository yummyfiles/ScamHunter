# ScamHunter Virtual Machine Safety Guide

A virtual machine (VM) can give research work a separate operating-system environment from your everyday setup. It's an extra layer of protection, not a guarantee that malware can't escape.

## What a VM is for

- Opening ordinary research tools in a separate environment.
- Testing suspicious files only when there is a legitimate need and a safe, controlled analysis setup.
- Keeping research changes separate from your everyday files and accounts.
- Reverting to a known clean snapshot after routine testing.

**Don't assume a VM makes every activity safe.** If all you need is to document a public threat-intelligence report, you usually don't need to download or execute anything.

## Suggested setup

Choose a reputable hypervisor supported by your host OS:

- [VirtualBox](https://www.virtualbox.org/) — widely used desktop virtualization.
- [KVM/QEMU](https://www.qemu.org/) — Linux virtualization options; KVM is integrated with the Linux kernel.
- [GNOME Boxes](https://apps.gnome.org/Boxes/) — a simpler desktop interface for QEMU/KVM.

Use an operating system image from its official publisher, keep the host and hypervisor updated, and create a clean baseline before research.

## Isolation checklist

Before using a VM for suspicious material:

- [ ] Take a clean snapshot before the test.
- [ ] Disable shared folders and drag-and-drop.
- [ ] Disable shared clipboard integration.
- [ ] Avoid USB passthrough and access to host devices.
- [ ] Don't sign in to personal accounts or store personal credentials in the VM.
- [ ] Keep host software and the guest OS patched.
- [ ] Consider whether networking is necessary at all. For unknown malware, default to no network unless the analysis environment is specifically designed for controlled network observation.
- [ ] If networking is required, use a deliberately isolated lab network—not your normal home LAN—and understand what traffic can still reach.
- [ ] Keep research notes and evidence separate from personal files.
- [ ] Revert to the clean snapshot or destroy the disposable VM after the task.

## Important limits

- Snapshots are not backups of everything and do not stop an escape vulnerability.
- NAT is not the same as full isolation; a guest may still reach the internet and sometimes other local services.
- A VPN or Tor connection does not make malware execution safe.
- Public analysis services may share submitted samples, URLs, and results. Don't submit confidential or personal material without understanding the policy.
- Don't test against real people's accounts, devices, or services without explicit authorization.

## Safer research order

1. Start with public threat feeds and existing analysis reports.
2. Record the source, timestamp, indicator type, and confidence.
3. Only if there's a clear need, consider analysis in a disposable, carefully isolated environment.
4. Document what the evidence supports and what remains unknown.

For ScamHunter, the default should be **passive research first**. A VM is an extra safety layer for cases that genuinely need it—not a reason to interact with dangerous sites or execute unknown files.
