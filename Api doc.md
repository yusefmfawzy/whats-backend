# Django Backend API Endpoints - WhatsApp Sales Chat System

This README file contains comprehensive details of all backend API endpoints required for the WhatsApp Sales Chat System built using Django and Django REST Framework.

## Table of Contents
- [Authentication](#authentication)
- [User Management](#user-management-admin-only)
- [Customer Management](#customer-management)
- [Assignment Management](#assignment-management)
- [Messaging](#messaging)
- [Webhook for Meta WhatsApp API](#webhook-for-meta-whatsapp-api)
- [WebSocket (Real-Time Chat)](#websocket-real-time-chat)

---

## Authentication
- **Login**: `POST /api/auth/login/`
- **Logout**: `POST /api/auth/logout/`
- **Get User Profile**: `GET /api/auth/me/`

## User Management (Admin only)
- **List Users**: `GET /api/users/`
- **Create User**: `POST /api/users/`
- **Get User Details**: `GET /api/users/<id>/`
- **Update User**: `PUT /api/users/<id>/`
- **Delete User**: `DELETE /api/users/<id>/`

## Customer Management
- **List Customers**: `GET /api/customers/`
- **Create Customer**: `POST /api/customers/`
- **sales can add name and notes**: `PUT /api/customers/<id>/`
- **Delete Customer**: `DELETE /api/customers/<id>/`

## Assignment Management
- **Assign Salesperson**: `POST /api/assignments/`
- **List Assignments**: `GET /api/assignments/`
- **Customer Assignment History**: `GET /api/customers/<id>/assignments/`

## Messaging
- **List All Messages**: `GET /api/messages/`
- **Send New Message**: `POST /api/messages/`
- **Get Specific Message**: `GET /api/messages/<id>/`
- **Customer Message History**: `GET /api/customers/<id>/messages/`

### Message Types
- Text
- Audio
- Video
- Image

## Webhook for Meta WhatsApp API
- **Webhook Verification (Meta setup)**: `GET /api/webhook/`
- **Handle Incoming WhatsApp Messages**: `POST /api/webhook/`

## WebSocket (Real-Time Chat)
- **WebSocket Connection**: `ws://<your-domain>/ws/chat/<customer_id>/`

### Authentication Method
- JWT-based authentication (access tokens required for API requests)

---

For any additional information or clarification, please contact the backend development team.
