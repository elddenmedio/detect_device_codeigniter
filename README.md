# detect_device_codeigniter
device detector (smarthphones/tablets)

This method can detect as many smathphones devices as you add

# First
Download this user_agent.php and replace it for you application/config/user_agent.php
This array is incomplete.

# Example
<code>
$this->load->library('user_agent');
</code>
<code>
if ($this->agent->is_browser()){
</code>
<code>
    $agent = $this->agent->browser().' '.$this->agent->version();
</code>
<code
}
</code>
elseif ($this->agent->is_mobile()){
    $agent = $this->agent->mobile();
}

else{
    $agent = 'Unidentified User Agent';
}

echo $agent;

echo $this->agent->platform(); // Platform info (Windows, Linux, Mac, etc.) if is smpthphone (Google Pixel, Samsum Galaxy S5, Samsung J7 Metal, etc)
</code>
