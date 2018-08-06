**Request:**

`curl "http://mobility-marketplace-test.here.com/demand.v1.s2s/offers?user_id=1&route.pickup.point.lat=32.1981&route.pickup.point.lng=34.8824&route.pickup.address=zarhin%2013&route.destination.point.lat=32.1981&route.destination.point.lng=34.8824&route.destination.address=zarhin%2013&constraints.passengers_no=1&constraints.suitcases_no=1&constraints.wheelchair=false&constraints.childs_seats=0&price_range.from_amount=10&price_range.to_amount=20&price_range.currency_code=USD&sort_type=1" -H "Authorization: Bearer eyJhbGciOiJub25lIiwidHlwIjoiSldUIn0.eyJzdWIiOiIxIiwiaXNzIjoicmVzdC1hc3N1cmVkIiwiZXhwIjoxNjQ0ODM4MTM2fQ.`"


**Response:**

    {
    "offers": [
    {
    "offer_id": "5a8c48479b1d4c0001bf20cd",
    "supplier": {
    "english_name": "tentacruel",
    "local_name": "tentacruel",
    "phone_number": "+9720516219186",
      },
    "estimated_pickup_time": "2018-02-20T16:13:31Z",
    "estimated_price_range": {
    "range": {
    "from_amount": "11",
    "to_amount": "97",
    "currency_code": "EUR"
    }
    },
    "offer_expiration_time": "2018-02-20T16:14:43Z",
    "cancellation_policy": "NOT_ALLOWED"
    },
    {
    "offer_id": "5a8c48479b1d4c0001bf20ca",
    "supplier": {
    "english_name": "shellder",
    "local_name": "shellder",
    "phone_number": "+9720538136208",
     },
    "estimated_pickup_time": "2018-02-20T16:13:36Z",
    "estimated_price_range": {
    "range": {
    "from_amount": "45",
    "to_amount": "88",
    "currency_code": "NIS"
    }
    },
    "offer_expiration_time": "2018-02-20T16:14:43Z",
    "cancellation_policy": "ALLOWED"
    }
    ]
    }
