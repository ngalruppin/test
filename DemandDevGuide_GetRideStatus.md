# HERE Demand API Workflow: *Getting a Ride's Status* #

**Ride** objects have different status values throughout the ride's "lifetime", depending on whether a driver has been assigned, whether the passenger has been picked up, and so on. See [Ride States and Transitions
](DemandDevGuide_RideStates.md) for a complete list of ride statuses.

The client application can poll periodically to get the current ride status, for example in order to display it to the end user.

**To get the current ride status:**

Call *GetRide*, passing the **ride_id** value that you received as a response to *CreateRide*. This returns a **Ride** object that contains several ride details, including the ride's status.

----
<details>
<summary><b>REST Example</b></summary>

**Request:**


    curl "http://mobility-marketplace-test.here.com/demand.v1.s2s/rides/5a8c484836bb08000157c180" -H "Authorization: Bearer eyJhbGciOiJub25lIiwidHlwIjoiSldUIn0.eyJzdWIiOiIxIiwiaXNzIjoicmVzdC1hc3N1cmVkIiwiZXhwIjoxNjQ0ODM4MTM2fQ."

**Response:**

	{
	    "user_id": "1",
	    "ride_id": "5a8c484836bb08000157c180",
	    "prebook_pickup_time": "2018-02-07T14:07:12Z",
	    "booking_estimated_price": {
	        "range": {
	            "from_amount": "11",
	            "to_amount": "97",
	            "currency_code": "EUR"
	        }
	    },
	    "status_log": {
	 	  "create_time": "2018-02-20T16:00:36Z",
	 	  "last_update_time": "2018-02-20T16:02:11Z",
	        "current_status": "DRIVER_EN_ROUTE",
	        "prev_statuses": [
	{
	                "status": "DRIVER_ASSIGNED",
	                "timestamp": "2018-02-20T16:02:06Z"
	            },
	
	            {
	                "status": "ACCEPTED",
	                "timestamp": "2018-02-20T16:00:46Z"
	            },
	            {
	                "status": "PROCESSING",
	                "timestamp": "2018-02-20T16:00:36Z"
	            }
	        ]
	    },
	    
	"supplier": {
	        "english_name": "tentacruel",
	        "local_name": "tentacruel",
	        "phone_number": "+9720516219186",
	        "address": "Not yet supported"
	    },
	    "passenger": {
	        "name": "asdasdasdasd",
	        "phone_number": "+9725326589",
	        "photo_url": "http://asdasdasdasdasd"
	    },
	    "passenger_note": "north side of the road"
	    "driver": {
	        "name": "Charmander",
	        "phone_number": "9010103",
	        "photo_url": "picture.url.here.com",
	        "driving_license_id": "5032147"
	    },
	    "vehicle": {
	        "license_plate_number": "75051046",
	        "vehicle_type": "STANDARD",
	        "make": "Kia",
	        "model": "model",
	        "color": "Red"
	    }
	}
 

</details>

----

<details>
<summary><b>GRPC Example</b></summary>

**Request:**

    COMING SOON


**Response:**

    COMING SOON

</details>


