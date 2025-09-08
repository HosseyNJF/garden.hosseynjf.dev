---
{"publish":true,"created":"2024-12-13 23:11","modified":"2025-09-08T10:23:01.096+02:00","cssclasses":""}
---


> A new interface for service layer using [[3. Resources/DRF\|DRF]] serializers and view mixins

# Core Idea

Decouple the service layer from your APIs, while using DRF's serializers to easily integrate with it and also allow internal calls.

# What is it?

Having a service layer that you may expose both via REST APIs and to other internal services is challenging, especially making sure that the input and output structure remains the same.

It consists of a middle layer that define their input and output types as serializers and assign them to their class variables, and multiple mixins that you can implement in your views and have them automatically use those serializers and interactions.

# Problems being solved

1. Interoperability between API and Internal
2. Separation of responsibility

# TODO

- Pagination
- Rate-limit in interaction layer
- Other commonly used patterns in DRF
