# Promo API - Reference

## Overview
RESTful API for managing promotional campaigns and offers.

## Endpoints
| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | /api/promos | List all promotions |
| POST | /api/promos | Create promotion |
| GET | /api/promos/:id | Get promotion details |
| PUT | /api/promos/:id | Update promotion |
| DELETE | /api/promos/:id | Delete promotion |
| POST | /api/promos/:id/validate | Validate promo code |

## Promo Object
| Field | Type | Description |
|-------|------|-------------|
| id | string | Unique identifier |
| code | string | Promo code |
| discount | number | Discount percentage |
| validFrom | date | Start date |
| validTo | date | Expiry date |
| maxUses | number | Maximum redemptions |
| usedCount | number | Times redeemed |

## Setup
```bash
npm install
cp .env.example .env
npm run dev
```