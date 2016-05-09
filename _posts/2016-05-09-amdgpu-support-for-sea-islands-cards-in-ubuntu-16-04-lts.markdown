---
published: false
title: AMDGPU support for Sea Islands cards in Ubuntu 16.04 LTS
layout: post
---
Sea Islands support for AMDGPU is not enabled by default in LK builds. Instead, it is a configuration parameter in the build process. This is due to it being highly experimental so far, with high potential for bugs (the GCN 1.1 implementation is incomplete, frankly, due to them focusing on newer cards).

After feeling the intense desire to try out AMDGPU in my own machine with a Sea Islands card, I scoured the internet for a custom Ubuntu 16.04 LTS kernel with Kabini (my APU generation) enabled, to no avail. So I decided, screw it, I'm gonna build my own.

Attached is a fully-working kernel + source git repository for Ubuntu 16.04, with AMDGPU kernel-space driver enabled by default. This will probably not be up to date, so if you can, just build it from my fork.