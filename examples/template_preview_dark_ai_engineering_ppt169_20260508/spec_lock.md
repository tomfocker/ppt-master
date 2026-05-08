# Execution Lock

> Machine-readable execution contract. Executor MUST read this before every SVG page. Values NOT listed here must NOT appear in SVGs.

## canvas
- viewBox: 0 0 1280 720
- format: PPT 16:9

## colors
- background: #0B1020
- panel: #0F172A
- secondary: #111827
- primary: #58A6FF
- accent: #22D3EE
- warning: #F59E0B
- danger: #F97373
- success: #34D399
- muted: #8B9BB4
- line: #243044
- text: #FFFFFF

## typography
- font_family: PingFang SC, Microsoft YaHei, Arial, sans-serif
- title: 48
- subtitle: 22
- heading: 26
- body: 16
- small: 12

## icons
- style: geometric inline symbols only

## images
- use: none

## page_rhythm
- 01_cover: anchor
- 02_architecture: dense
- 03_risk_matrix: dense
- 04_metrics: dense
- 05_close: breathing

## forbidden
- rgba()
- <style>, class, <foreignObject>, textPath, @font-face, <animate*>, <script>, <iframe>, <symbol>+<use>
- <g opacity> (set opacity on each child element individually)
