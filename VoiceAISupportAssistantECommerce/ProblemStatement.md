# Voice AI Support Assistant (E-commerce Returns)**

## **Objective**

Build a system that takes a **voice query** and returns a **text + voice response**.

---

## **Problem Statement**

Design a **voice-enabled support assistant for an e-commerce platform (returns & orders)**.

The system should:

1. Accept a user query as audio
2. Convert speech → text
3. Generate a response using an LLM
4. Convert the response back to speech
5. Return both text and audio

The assistant should handle queries such as:

* “Where is my order?”
* “I want to return a product”
* “What’s your refund policy?”

You will be provided with a **fixed dataset of orders and policies**.
Your system should use this data to answer queries.

---

## **Requirements**

* Input: audio file
* Output: text + synthesized audio
* Interface: CLI, API, or simple UI
* Use the provided dataset as the source of truth

---

## **Notes**

* The problem is intentionally open-ended
* Make and document reasonable assumptions

---

## **Deliverables**

* Code repository
* README with:

  * setup
  * assumptions
  * design decisions & tradeoffs
  * improvements

---

## **Evaluation Criteria**

* Execution speed
* Code quality
* Git hygiene
* Problem understanding, clarity in terms of assumptions and decisions
* Use of AI tools, 3rd party api services

---

## **Constraints**

* Any tools allowed (including AI)

---

## **Submission**

Repo link

---

# **Dataset**

You can give this as a simple JSON file.

## **orders.json**

```json
[
  {
    "order_id": "ORD123",
    "user_id": "U1",
    "status": "delivered",
    "item": "Wireless Headphones",
    "delivery_date": "2026-03-20",
    "return_window_days": 7
  },
  {
    "order_id": "ORD124",
    "user_id": "U1",
    "status": "in_transit",
    "item": "Running Shoes",
    "expected_delivery": "2026-03-30"
  },
  {
    "order_id": "ORD125",
    "user_id": "U2",
    "status": "delivered",
    "item": "Smart Watch",
    "delivery_date": "2026-03-10",
    "return_window_days": 7
  }
]
```

---

## **policies.json**

```json
{
  "returns": {
    "allowed": true,
    "window_days": 7,
    "conditions": [
      "Item must be unused",
      "Original packaging required"
    ]
  },
  "refunds": {
    "method": "original payment method",
    "processing_time_days": 5
  },
  "support_hours": "9 AM - 6 PM IST"
}
```
---
Feel free to add more details to the dataset depending on your implementation.

