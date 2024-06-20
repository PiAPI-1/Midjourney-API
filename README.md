# Midjourney-API
Integrate our unofficial [Midjourney API](https://piapi.ai/midjourney-api) to build your AIimage applications - providing your users with infinitepossibilities generating images from text inputs.
<br><br>
<div align="center" max-width: 100%>
  <img src="https://iili.io/dHoZEtp.md.png"/>
</div>
<br><br>
<h2>Features</h2>
<ol>
  <li>Built-in Load Balancer</li>
  <li>Connect Multiple Accounts</li>
  <li>Complete access to all endpoints</li>
  <li>Workspace and Webhook</li>
  <li>Supports V6, sref and cref</li>
  <li>Midjourney Subscription Excluded</li>
</ol>
<br><br>
<h2>Supported Operations</h2>
<ul>
  <li>Imagine - A single prompt generating 4 images in 2x2 grid</li>
  <li>Upscale - Enhance the image quality with Midjourney’s upscaler</li>
  <li>Variation - Create variants of the selected image</li>
  <li>Describe - Provide descriptive texts for the image submitted</li>
  <li>Blend - Combine two images into a new and original image</li>
  <li>Inpaint - Change parts of the submitted image</li>
  <li>Zoom - Extend the selected image beyond original boundary</li>
  <li>Pan - Expand the image towards a chosen direction</li>
  <li>--sref - Preserve consistency through style reference</li>
  <li>--cref - Create images of the same character in different scenes</li>
</ul>
<br><br>
<h2>Supported Modes</h2>
<ul>
  <li>Relax Mode</li>
  <li>Fast Mode</li>
  <li>Turbo Mode</li>
</ul>
<br><br>
<h2>Usage Options</h2>
<h3>Pay-as-you-go Option</h3>
<p>All you need to do is sign-up, purchase credits in our Workspace and you can use our API right away! 
  The service uses PiAPI’s Midjourney account pools, so you don’t have to worry about their operation at all!
  <br><br>
  Please refer to our <a herf="https://piapi.ai/pricing">pricing page</a> for more information.
</p>
<ul>
  <li>Don't need your own Midjourney account(s) pool!</li>
  <li>Don't need to manage/operate Midjourney accounts</li>
  <li>Complete access to all endpoints</li>
  <li>Get started with integrating the API right away!</li>
</ul>
<h4>Pricing</h4>
<ul>
  <li>Relax Mode: <b>$0.015</b>/imagine task</li>
  <li>Fast Mode: <b>$0.045</b>/imagine task</li>
  <li>Turbo Mode: <b>$0.10</b>/imagine task</li>
</ul>
<br>
<h3>Host-your-account Option</h3>
<p>With our Host-Your-Account service, you will be using your own Midjourney Account(s) and 
  you will be required to buy PiAPI Midjourney API seat(s), bind your Midjourney Account(s) to the seat(s), and you are ready to go!!
  <br><br>
</p>
Please refer to our <a herf="https://piapi.ai/pricing">pricing page</a> for more information. 
<ul>
  <li>Already have your own Midjourney account(s)?</li>
  <li>Don't want to wait in queue for other's tasks to be completed?</li>
  <li>Offers overall faster generation time!</li>
</ul>
<h4>Flat Pricing</h4>
<ul>
  <li><b>$8</b>/seat/month</li>
</ul>
<br>
<h2>Usage Options</h2>
<h3>Pay-as-you-go Option</h3>
<ul>
  <li>Register for PiAPI's Workspace using your GitHub account.</li>
  <li>Obtain your API KEY from our <a herf="https://app.piapi.ai/">Workspace</a></li>
  <li>Start coding right away!</li>
</ul>
<br>
<h4>Sample API Calls (using cURL)</h4>
<br>
<p>Creating an imagine call</p>

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
<p>Returning</p>

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
<p>Returning</p>
Check out our <a herf-"https://piapi.ai/docs/midjourney-api/fetch">documentation</a> for more information!
<br>
<br>
<h2>Contact us</h2>
<p>Email: contact@piapi.ai</p>
