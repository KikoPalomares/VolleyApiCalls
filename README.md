# VolleyApiCalls
Llamadas API en android usando Volley con Kotlin

https://kikopalomares.com

```kotlin
        // Instantiate the RequestQueue.
        val queue = Volley.newRequestQueue(this)
        val url = "https://kikopalomares.com"
        // Request a string response from the provided URL.
        val stringRequest = StringRequest(url,
                Response.Listener<String> { response ->
                    // Display the first 100 characters of the response string.
                    Log.i(LOG_TAG, "Response is: ${response.substring(0, 100)}")
                },
                Response.ErrorListener { error ->
                    error.printStackTrace()
                    Log.e(LOG_TAG, "That didn't work!")
                })

        // Add the request to the RequestQueue.
        queue.add(stringRequest)
```

Puedes ver el video donde se explica como hacer este codigo: https://youtu.be/mJYwYc51IKI
