# Execution Lock

> Machine-readable execution contract. Executor MUST read this before every SVG page.

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
- title: 52
- heading: 26
- body: 16
- small: 12

## images
- cover_bg: images/cover_bg.png
- content_bg: images/content_bg.png

## page_rhythm
- 01_cover: anchor
- 02_architecture: dense
- 03_metrics: dense

## forbidden
- rgba()
- <style>, class, <foreignObject>, textPath, @font-face, <animate*>, <script>, <iframe>, <symbol>+<use>
- <g opacity> (set opacity on each child element individually)
