# Build-a-PowerPoint-Generator-AI-Agent-with-LLMs

PowerPoint Generator with Google Gemini is a Python-based tool that automatically creates well-structured PowerPoint presentations from a topic using Google’s Gemini API and optional images from Pexels.

## Project overview
### Goal: 
Generate complete .pptx presentations from a single topic prompt, including slide titles, bullet content, and optional images
### Core idea:
Use Gemini to draft a JSON outline of slides, then render slides with python-pptx, falling back to a predefined outline if the API quota or JSON parsing fails.
## Features
Automatic slide outline generation (title, content, slide_type) via Gemini (gemini-2.5-pro).
Fillback outline with intro, background, key concepts, applications, and conclusion when Gemini is unavailable.
​Title, content, and image slides with consistent typography and layout using python-pptx.
​Optional image enhancement per slide: Gemini suggests a short image description, and a relevant photo is fetched from the Pexels API (with placeholder fallback).
