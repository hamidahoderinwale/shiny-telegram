<!-- YourComponent.svelte -->
<script>
    import PdfViewer from 'svelte-pdf'; // Import PDF viewer component
    
    let src = 'https://images.squarespace-cdn.com/content/v1/5a7cb549e5dd5b79d078323c/1518798855670-Y949V7PJR82336LGLMOR/B21-231.jpg?format=500w';
    let altText = 'Building21';
    let pdfUrl = 'file:///Users/hamidahoderinwale/Downloads/Notes%20on%20Archive%20Fever%5B65%5D.pdf';
    let showModal = false;

    function openModal() {
        showModal = true;
    }
</script>

{#if showModal}
    <div class="modal">
        <div class="modal-content">
            <span class="close" on:click={() => showModal = false}>&times;</span>
            <PDFViewer src={pdfUrl} />
        </div>
    </div>
{/if}

<nav>
    <a href="/">Home</a>
    <a href="src/projects.svelte">Projects</a>
</nav>

<h1 class="font-size: 1rem;">Learnathon</h1>
<p>2/2024</p>
<br>
<p>A learning sprint. <a href="https://www.rabbitholeathon.com/" target="_blank">Focused rabbit-holes (in a sprint?)</a>. Something new that's a little more familliar...</p>
<br>
<p>The Learnathon is a chance to finally dive deep into a topic that piqued your curiosity, but you never pursued; a problem you’re itching to solve; or an issue you’re trying to make sense of. It’s a space to spend a few concerted hours exploring a new topic, subject, or idea. </p>
<br>

<p> Running Learnathons are really easy. If you do run one, I think it's important to set the scene for what to do. An email was sent out about a week in advance, so people could think about what they might do, collect resources, etc.</p><br>
<p>Learning is ominous. Deliverables are great! A blog post, a written-out-proof, some slightly less buggy code.</p>
<br><p>Whatever it is, learning by doing is supreme. But, it's also reasonable and encouraged to just try and understand whatever it is you want to wrap your mind around (that's what I did!). A slightly-complex research paper is a great start, especially if it's related to other work you're trying to accomplish. </p>
<br>
<hr>
<br>
<img src={src} alt='{altText}!'>
<br>
<em><p><a href="https://building21.ca/" target="_blank" class="selection:bg-purple-300 selection:text-purple-900">Building21</a> graciously supported the event. The initial inspiration for running this was a <a href="https://firelight-mit.github.io/" target="_blank">friend's club</a> at his school.</p></em>
<br>
<p>Here's the structure we followed:</p>
<div class="structure">
    <li>15 minute pre-amble</li>
    <li>1 hour work time</li>
    <li>15 minute breaktime</li>
    <li>1 hour work time</li>
    <li>15+ minute debrief</li>
</div>
<p>In total it was a 2 hour and 45 minute event.<p>
<br>
<p>Note that the time frame is super short! It was nice. You build enough momentum that you can continue if you'd like. If not, it's a nice boost of motivation to do something else. But, at least you did something! This is probably the most valuable takeaway. Just do something.</p>
<br>
<h3>Cool stuff people learned and worked on</h3>
<br> 
<p>People did chemistry (crystallography!); first-order logic; messed around with code; caught up on reading; researched thyroid imbalances, <button on:click={openModal}>Library Cataloguing</button>, and <a data-sveltekit-preload-data="hover" href="src/projects.svelte" class="max-w-xl selection:bg-purple-300 selection:text-purple-900">more</a>.</p>
<br>
<p>Overall, it was really great to run (albeit I didn't have to actually do that much). People are usually excited to talk about things that excite them. This is a fun catalyst for great conversations too.</p>
<br>
<p>The most notable thing was just how the mood changed. Co-working sessions are great, but I think there's this pressure to have something to talk about by the end, so you just end up actually trying. There's nothing concrete to display, so you just get guided ramblings (which is really dope).</p>
<br>
<p>In short, run one!</p>
