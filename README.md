eee — encrypted P2P chat + file sharing

No servers, no accounts, no dependencies.

## Install

macOS / Linux / WSL:
  curl -sSL https://github.com/wildneuro/eee-releases/releases/latest/download/install.sh | bash

Windows (PowerShell):
  iwr -useb https://github.com/wildneuro/eee-releases/releases/latest/download/install.ps1 | iex

## Features

- End-to-end encrypted (AES-256-GCM)
- P2P via libp2p (DHT + mDNS + relay + hole-punching)
- File sharing with ASCII image preview
- Privacy mode (message masking, default on)
- Screen recording detection + kill
- Audio notifications on send/receive
- Auto-update on startup
- Cross-platform: macOS, Linux, Windows (amd64 + arm64)
- Single binary, no runtime dependencies

## Usage

  eee                        TUI: generate or enter a shared secret key
  eee <64hex>                skip key entry, join with a shared key
  eee listen                 headless mode (print key + PeerID)
  eee connect <PeerID> <key> headless connect
  eee remove                 uninstall

In TUI chat:
  /send <path>   send a file (or drag-drop file into terminal)
  /accept        accept incoming file
  /decline       decline incoming file
  /preview       preview image before accepting
  /privacy       toggle message masking
  /new           new session (new key)
  /update        check and apply updates
  /help          show available commands
  /quit          exit

## Latest release: v0.3.12

Binaries: https://github.com/wildneuro/eee-releases/releases/tag/v0.3.12
