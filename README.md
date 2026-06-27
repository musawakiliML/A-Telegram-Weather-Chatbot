# WhatsAppy SDK

> **The modern Python SDK for the Meta WhatsApp Cloud API.**

[![Python](https://img.shields.io/badge/python-3.10%2B-blue.svg)](#)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](#)
[![Status](https://img.shields.io/badge/status-active-success.svg)](#)

WhatsAppy SDK is an open-source, developer-first Python wrapper for the **Meta WhatsApp Cloud API**.

Instead of manually constructing HTTP requests and parsing deeply nested webhook payloads, WhatsAppy provides a clean, typed, and intuitive Python interface for building production-ready WhatsApp applications.

Whether you're building chatbots, customer support systems, AI assistants, ecommerce platforms, or internal business tools, WhatsAppy lets you focus on your application—not the API boilerplate.

---

[//]: # (## Why WhatsAppy_SDK?)

[//]: # ()
[//]: # (The existing Python libraries for WhatsApp Cloud API are often:)

[//]: # ()
[//]: # (- outdated)

[//]: # (- incomplete)

[//]: # (- thin wrappers around `requests`)

[//]: # (- tied to third-party providers)

[//]: # (- missing support for newer WhatsApp features such as Flows and Commerce APIs)

[//]: # ()
[//]: # (WhatsAppy is different.)

[//]: # ()
[//]: # (It is built directly on top of the official Meta WhatsApp Cloud API with one goal:)

[//]: # ()
[//]: # (> **Provide the best developer experience for Python developers.**)

[//]: # ()
[//]: # (---)

[//]: # ()
[//]: # (# Features)

[//]: # ()
[//]: # (### Messaging)

[//]: # ()
[//]: # (- Send text messages)

[//]: # (- Send images, videos, audio and documents)

[//]: # (- Send stickers)

[//]: # (- Send contacts)

[//]: # (- Send locations)

[//]: # (- Send reactions)

[//]: # (- Reply to messages)

[//]: # (- Mark messages as read)

[//]: # ()
[//]: # (### Interactive Messages)

[//]: # ()
[//]: # (- Reply buttons)

[//]: # (- Call-to-action buttons)

[//]: # (- Lists)

[//]: # (- Multi-product messages)

[//]: # (- Single-product messages)

[//]: # (- Catalog messages)

[//]: # (- Flow messages)

[//]: # ()
[//]: # (### Templates)

[//]: # ()
[//]: # (- Send template messages)

[//]: # (- Template parameter builders)

[//]: # (- Media templates)

[//]: # (- Authentication templates)

[//]: # ()
[//]: # (### Media)

[//]: # ()
[//]: # (- Upload media)

[//]: # (- Download media)

[//]: # (- Delete media)

[//]: # ()
[//]: # (### Webhooks)

[//]: # ()
[//]: # (- Automatic webhook verification)

[//]: # (- Typed webhook models)

[//]: # (- Event routing)

[//]: # (- Message parsing)

[//]: # ()
[//]: # (### Developer Experience)

[//]: # ()
[//]: # (- Fully typed API)

[//]: # (- Pydantic models)

[//]: # (- Sync and Async clients)

[//]: # (- Excellent documentation)

[//]: # (- Framework integrations)

[//]: # (- First-class testing support)

[//]: # ()
[//]: # (---)

[//]: # ()
[//]: # (# Installation)

[//]: # ()
[//]: # (```bash)

[//]: # (pip install whatsappy_sdk)

[//]: # (```)

[//]: # ()
[//]: # (---)

[//]: # ()
[//]: # (# Quick Start)

[//]: # ()
[//]: # (```python)

[//]: # (from whatsappy_sdk import WhatsApp)

[//]: # ()
[//]: # (client = WhatsApp&#40;)

[//]: # (    access_token="YOUR_ACCESS_TOKEN",)

[//]: # (    phone_number_id="YOUR_PHONE_NUMBER_ID")

[//]: # (&#41;)

[//]: # ()
[//]: # (client.messages.send_text&#40;)

[//]: # (    to="2348012345678",)

[//]: # (    text="Hello from WhatsAppy!")

[//]: # (&#41;)

[//]: # (```)

[//]: # ()
[//]: # (---)

[//]: # ()
[//]: # (# Webhook Example)

[//]: # ()
[//]: # (```python)

[//]: # (from fastapi import FastAPI)

[//]: # (from whatsappy_sdk import WebhookRouter)

[//]: # ()
[//]: # (app = FastAPI&#40;&#41;)

[//]: # ()
[//]: # (router = WebhookRouter&#40;&#41;)

[//]: # ()
[//]: # ()
[//]: # (@router.message&#40;&#41;)

[//]: # (async def handle_message&#40;message&#41;:)

[//]: # (    print&#40;message.text&#41;)

[//]: # ()
[//]: # ()
[//]: # (app.include_router&#40;router.fastapi&#40;&#41;&#41;)

[//]: # (```)

[//]: # ()
[//]: # (Simple.)

[//]: # ()
[//]: # (Clean.)

[//]: # ()
[//]: # (Pythonic.)

[//]: # ()
[//]: # (---)

[//]: # ()
[//]: # (# Project Goals)

[//]: # ()
[//]: # (WhatsAppy aims to become the most complete Python SDK for the Meta WhatsApp Cloud API by providing support for:)

[//]: # ()
[//]: # (- Messaging)

[//]: # (- Media)

[//]: # (- Templates)

[//]: # (- Commerce APIs)

[//]: # (- WhatsApp Flows)

[//]: # (- Business Profile Management)

[//]: # (- Phone Number Management)

[//]: # (- Webhook Routing)

[//]: # (- Async Support)

[//]: # (- Developer CLI)

[//]: # (- Testing Utilities)

[//]: # ()
[//]: # (---)

[//]: # ()
[//]: # (# Roadmap)

[//]: # ()
[//]: # (## v0.1)

[//]: # ()
[//]: # (- Core client)

[//]: # (- Authentication)

[//]: # (- Send text messages)

[//]: # (- Webhook verification)

[//]: # (- Typed models)

[//]: # (- FastAPI example)

[//]: # (- Flask example)

[//]: # (- Django example)

[//]: # ()
[//]: # (## v0.2)

[//]: # ()
[//]: # (- Interactive messages)

[//]: # (- Media API)

[//]: # (- Templates)

[//]: # (- Better webhook routing)

[//]: # ()
[//]: # (## v0.3)

[//]: # ()
[//]: # (- WhatsApp Flows)

[//]: # (- Commerce API)

[//]: # (- Catalog support)

[//]: # (- Product messages)

[//]: # ()
[//]: # (## v1.0)

[//]: # ()
[//]: # (- Complete Cloud API support)

[//]: # (- CLI)

[//]: # (- Plugin architecture)

[//]: # (- Production-ready documentation)

[//]: # (- 100% typed public API)

[//]: # ()
[//]: # (---)

[//]: # ()
[//]: # (# Philosophy)

[//]: # ()
[//]: # (WhatsAppy is built around three principles.)

[//]: # ()
[//]: # (## Developer Experience First)

[//]: # ()
[//]: # (The SDK should feel natural to Python developers.)

[//]: # ()
[//]: # (## Stay Close to Meta)

[//]: # ()
[//]: # (The SDK wraps the official WhatsApp Cloud API without introducing unnecessary abstractions.)

[//]: # ()
[//]: # (## Production Ready)

[//]: # ()
[//]: # (Everything included in WhatsAppy should be suitable for real-world applications.)

[//]: # ()
[//]: # (---)

[//]: # ()
[//]: # (# Documentation)

[//]: # ()
[//]: # (Documentation is currently under active development.)

[//]: # ()
[//]: # (It will include:)

[//]: # ()
[//]: # (- Getting Started)

[//]: # (- Creating a Meta App)

[//]: # (- Configuring WhatsApp Cloud API)

[//]: # (- Sending your first message)

[//]: # (- Receiving webhooks)

[//]: # (- Interactive messages)

[//]: # (- Templates)

[//]: # (- Flows)

[//]: # (- Commerce)

[//]: # (- Deployment guides)

[//]: # (- Best practices)

[//]: # ()
[//]: # (---)

[//]: # ()
[//]: # (# Examples)

[//]: # ()
[//]: # (Example projects will include:)

[//]: # ()
[//]: # (- Echo Bot)

[//]: # (- AI Chatbot)

[//]: # (- Customer Support Bot)

[//]: # (- Ecommerce Assistant)

[//]: # (- SilentPulse Integration)

[//]: # (- FastAPI)

[//]: # (- Flask)

[//]: # (- Django)

[//]: # ()
[//]: # (---)

[//]: # ()
[//]: # (# Contributing)

[//]: # ()
[//]: # (Contributions are welcome!)

[//]: # ()
[//]: # (Whether you're fixing bugs, improving documentation, adding new WhatsApp features, or suggesting API improvements, we'd love your help.)

[//]: # ()
[//]: # (Please open an issue before working on large features so we can discuss the design together.)

[//]: # ()
[//]: # (---)

[//]: # ()
[//]: # (# Inspiration)

[//]: # ()
[//]: # (WhatsAppy is inspired by the developer experience offered by projects such as:)

[//]: # ()
[//]: # (- FastAPI)

[//]: # (- Requests)

[//]: # (- HTTPX)

[//]: # (- Pydantic)

[//]: # (- SQLAlchemy)

[//]: # ()
[//]: # (The goal is to bring the same level of elegance and productivity to the Meta WhatsApp Cloud API.)

[//]: # ()
[//]: # (---)

[//]: # ()
[//]: # (# License)

[//]: # ()
[//]: # (MIT License.)

[//]: # ()
[//]: # (---)

[//]: # ()
[//]: # (## About the Project)

[//]: # ()
[//]: # (WhatsAppy started as an internal SDK built to power several production applications, including AI assistants, anonymous feedback systems, research tools, ecommerce platforms, and automation workflows.)

[//]: # ()
[//]: # (Rather than solving the same integration challenges repeatedly, the SDK was open-sourced to help the broader Python community build better WhatsApp applications with less effort.)

[//]: # ()
[//]: # (If WhatsAppy saves you time, consider giving the project a ⭐ on GitHub.)