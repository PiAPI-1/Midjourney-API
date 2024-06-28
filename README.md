# Midjourney API (Hassle-free Integration)
Enhance your AI-powered image applications with our unofficial [Midjourney API](https://piapi.ai/midjourney-api), providing users with unlimited potential to generate images from text prompts.
<br><br>
<img src="https://github.com/PiAPI-1/Midjourney-API/assets/173328932/f1424aa4-e96d-43e3-aa88-2b346c5e89e5" alt="screenshot of the Midjourney API page from PiAPI" width="95%"/>
<br><br>
<h2>Features</h2>
<ol>
  <li>Integrated Load Balancer</li>
  <li>Multi-Account Connectivity</li>
  <li>Full Endpoint Access</li>
  <li>Workspace and Webhook Support</li>
  <li>Compatible with V6, --sref, and --cref</li>
  <li>Midjourney Subscription Excluded</li>
  <li>Supported modes: Relax, Fast and Turbo</li>
</ol>
<br><br>
<h2>Supported Operations</h2>
<ul>
  <li>Imagine</li>
  <li>Upscale</li>
  <li>Variation</li>
  <li>Describe</li>
  <li>Blend</li>
  <li>Inpaint</li>
  <li>Zoom</li>
  <li>Pan</li>
  <li>--sref</li>
  <li>--cref</li>
</ul>

<br><br>

<h2>Usage Options</h2>

<h3>Pay-as-you-go Option</h3>

<p>
  To get started, simply sign up and purchase credits in our Workspace. Once done, you can immediately access our API! Our service leverages PiAPI’s Midjourney account pools, ensuring seamless operation without any hassle on your part.
</p>

<ul>
  <li>No need for your own Midjourney account(s) pool!</li>
  <li>No need to manage or operate Midjourney accounts</li>
  <li>Full access to all endpoints</li>
  <li>Start integrating the API immediately!</li>
</ul>

<br>

<h3>Host-your-account Option</h3>
<p>
  When you choose our Host-Your-Account service, you'll use your own Midjourney Account(s). Then you can subscribe to PiAPI's Midjourney API seat(s), connecting your Midjourney account(s) to the seat(s), and you're ready for integration!
</p>

<ul>
  <li>Faster generation time</li>
  <li>Supports hosting of multiple accounts</li>
  <li>Stable API service</li>
</ul>

<br>

<h3>Pricing</h3>
<h4>Pay-as-you-go Option</h4>
<ul>
  <li>Relax Mode: <b>$0.015</b>/imagine task</li>
  <li>Fast Mode: <b>$0.045</b>/imagine task</li>
  <li>Turbo Mode: <b>$0.10</b>/imagine task</li>
</ul>
<h4>Host-your-account Option</h4>
<ul>
  <li>Flat pricing: <b>$8</b>/seat/month</li>
</ul>
<br>
Please refer to our <a href="https://piapi.ai/pricing">pricing page</a> for more information. 
<br><br>
<h2>Usage Steps</h2>
<h3>Pay-as-you-go Option</h3>
<ul>
  <li>Register for PiAPI's Workspace using your GitHub account.</li>
  <li>Obtain your API KEY from our <a href="https://app.piapi.ai/">Workspace</a></li>
  <li>Start coding right away!</li>
</ul>
<br>
<h4>Sample API Calls (using cURL)</h4>
<br>
<p>Create an imagine call</p>

```
curl --location 'https://api.piapi.ai/mj/v2/imagine' \
--header 'X-API-Key: your_api_key_here' \
--header 'Content-Type: application/json' \
--data '{
  "custom_mode": false,
  "input": 
        {
            "gpt_description_prompt":"a nice car",
            "make_instrumental": false
        }
}'
```
<p>Response</p>

```
{
    "code": 200,
    "data": {
        "task_id": "record_this_taskID"
    },
    "message": "success"
}
```
<br>
<p>Fetch the imagine call</p>

```
curl --location 'https://api.piapi.ai/mj/v2/fetch' \
--header 'X-API-Key: your_api_key_here' \
--header 'Content-Type: application/json' \
--data '{
  "custom_mode": false,
  "input": 
        {
            "task_id": "Insert_the_taskID_here"
        }
}'
```
<br>
<p>Response - Check out our <a href="https://piapi.ai/docs/midjourney-api/fetch">documentation</a> for more information!</p>
<br>
<br>
<h2>Contact us</h2>
<p>Email: <a href="mailto:contact@piapi.ai">contact@piapi.ai</a></p>
<br>
