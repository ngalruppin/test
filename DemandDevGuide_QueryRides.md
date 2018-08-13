# HERE Demand API Workflow: *Querying for Rides* #

You can query for rides according to their status and the time they were last updated. 

**To query for a ride by status and/or update time:**

Call *GetRideListRequest*.

>**Note:** This call is identical for the C2S and S2S APIs. However, for the C2S call, only the single current user's rides are returned; for the S2S call, all users' rides that match the filter are returned.

----
<details>
<summary><b>REST Example</b></summary>

**Request:**

    COMING SOON

**Response:**

	COMING SOON

</details>

----

<details>
<summary><b>GRPC Example</b></summary>

**Request:**

    COMING SOON


**Response:**

    COMING SOON

</details>

----

**S2S Only: To query for a ride by user ID and by status and/or update time:**

Call *GetRideListByUserRequest*, passing the ID of the user whose rides you want to retrieve.

----
<details>
<summary><b>REST Example</b></summary>

**Request:**

    COMING SOON

**Response:**

	COMING SOON

</details>

----

<details>
<summary><b>GRPC Example</b></summary>

**Request:**

    COMING SOON


**Response:**

    COMING SOON

</details>

----


**S2S Only: To query for rides by last update time:**

Call *GetRecentRidesRequest*, passing the minimum update time with which you want to filter the results. If no minimum time is sent, a default of the last two hours is used.

----
<details>
<summary><b>REST Example</b></summary>

**Request:**

    COMING SOON

**Response:**

	COMING SOON

</details>

----

<details>
<summary><b>GRPC Example</b></summary>

**Request:**

    COMING SOON


**Response:**

    COMING SOON

</details>

----