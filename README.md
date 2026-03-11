# Jewellens AI Platform 💎

An AI-powered jewelry discovery and recommendation platform that allows
users to explore jewelry collections using intelligent search and visual
retrieval.

This project combines **AI-based image embeddings, vector similarity
search, and a modern web interface** to help users browse jewelry items
like rings and necklaces.

------------------------------------------------------------------------

# Project Overview

Jewellens AI Platform is a full-stack application consisting of:

-   **Frontend**: React + Vite web interface
-   **Backend**: FastAPI server
-   **AI Retrieval System**: CLIP embeddings + FAISS vector search
-   **Dataset**: Jewelry catalog images

The platform allows users to:

-   Browse jewelry collections
-   Search jewelry intelligently
-   View item details
-   Add items to cart or wishlist

------------------------------------------------------------------------

# Features

## Jewelry Catalog

Users can explore the full jewelry collection including:

-   Rings
-   Necklaces

Items are dynamically loaded from the backend API.

## Smart AI Retrieval

The system uses:

-   **CLIP Vision Transformer**
-   **FAISS Vector Search**

to retrieve visually similar jewelry.

## Product Details

Each item includes:

-   Name
-   Material
-   Style
-   Price
-   Collection
-   Hallmark
-   Purity

## Wishlist and Cart

Users can:

-   Add jewelry to cart
-   Add items to wishlist
-   View selected items

## Responsive UI

The application provides a modern luxury-style interface optimized for
browsing jewelry.

------------------------------------------------------------------------

# Tech Stack

## Frontend

-   React
-   Vite
-   JavaScript
-   CSS

## Backend

-   FastAPI
-   Python
-   Uvicorn

## AI & Retrieval

-   SentenceTransformers CLIP Model
-   FAISS Vector Database
-   HuggingFace Transformers

## Other Libraries

-   NumPy
-   Pillow
-   Requests

------------------------------------------------------------------------

# Project Structure

    Jewellens-AI-Platform
    │
    ├── backend
    │   ├── main.py
    │   ├── api routes
    │   └── requirements.txt
    │
    ├── frontend
    │   ├── src
    │   │   ├── components
    │   │   ├── pages
    │   │   └── main.jsx
    │   ├── index.html
    │   └── package.json
    │
    ├── Jewelry_RAG
    │   ├── data
    │   ├── jewelry.index
    │   ├── jewelry_visual.index
    │   └── jewelry_hybrid.index
    │
    ├── run_backend.bat
    └── README.md

------------------------------------------------------------------------

# How to Run the Project

## 1 Install Requirements

Ensure you have:

-   Python 3.10+
-   Node.js
-   Git

------------------------------------------------------------------------

# Backend Setup

Navigate to project root and run:

``` bash
pip install -r backend/requirements.txt
```

Run the backend:

``` bash
run_backend.bat
```

or manually:

``` bash
uvicorn backend.main:app --reload
```

Backend will start at:

    http://localhost:8000

------------------------------------------------------------------------

# Frontend Setup

Open a new terminal and run:

``` bash
cd frontend
npm install
npm run dev
```

Frontend will start at:

    http://localhost:3000

------------------------------------------------------------------------

# Reset / Delete Existing User Data

If you want to register a new user, delete the stored user database.

Steps:

1.  Navigate to backend storage folder
2.  Delete the database file (example):

```{=html}
<!-- -->
```
    users.db

Then restart the backend.

The application will allow new user registration.

------------------------------------------------------------------------

# How to Use the Application

1 Open the website

    http://localhost:3000

2 Register a user

3 Browse jewelry collections

4 Click an item to view details

5 Add items to cart or wishlist

6 Explore necklaces and rings categories

------------------------------------------------------------------------

# AI Working Flow

The AI retrieval system works as follows:

1 User loads jewelry catalog

2 Jewelry images are embedded using CLIP

3 Embeddings are stored in FAISS vector index

4 When a search happens:

-   Query is converted into embedding
-   Similar vectors are retrieved
-   Top matches are returned

5 Frontend displays results.

------------------------------------------------------------------------

# Future Improvements

Possible enhancements:

-   Voice-based jewelry search
-   Image upload search
-   Recommendation engine
-   Payment gateway
-   User profiles
-   Cloud deployment

------------------------------------------------------------------------

# Author

Developed as an AI-powered jewelry exploration platform demonstrating:

-   Vector similarity search
-   AI image retrieval
-   Full stack web development
