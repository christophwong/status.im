---
id: open_positions
title: Open Positions
description: Check out our open positions.
---

# Open Positions

Please note that all of our positions are remote - we welcome contributors from all over the globe. Want to chat to our People Ops team? Drop by the [#hiring](https://discord.gg/ncDjzk2) channel on our community Discord, or check out the latest project discussions over at [discuss.status.im](https://discuss.status.im) :) 
 
<script type="application/javascript">
  /* If Job ID is provided modify iframe to show specific job */
  const openSpecificJobPage = () => {
    const urlParams = new URLSearchParams(window.location.search);
    const gh_jid = urlParams.get('gh_jid')
    if (gh_jid !== undefined) {
      let iFrame = document.getElementById('greenhouse-job-board');
      const url = `https://boards.greenhouse.io/status72/jobs/${gh_jid}`
      if (iFrame.src != url) { /* avoid reloading loop */
        console.log(`Opening: ${url}`)
        iFrame.src = url
      }
    }
  }
</script>
<div class="my-12">
<div class="col-span-1"></div>
<iframe id="greenhouse-job-board" class="col-span-2 xl:col-span-4" onload="openSpecificJobPage();" height="600em" width="100%" src="https://boards.greenhouse.io/status72"  title="GreenHouse Job Board"></iframe>
</div>

If you believe you can contribute, but don't see a role that closely matches your skills - please send a short note and your CV to talent@status.im.
