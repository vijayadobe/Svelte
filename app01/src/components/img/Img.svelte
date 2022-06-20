<script>
    const  url = "https://api.balarammullick.com/ProdImage/d3e0be0f-80a9-4d55-90c0-9cd15af536af.jpg";
    const btnState = true
    import EmotionCss from "../emotion-css/emotion-css.svelte";
  </script>
  
  
  
  <section>
      <h5> Displaying an Image</h5>
      <img src={url}  alt="sweets" />
      <p> Image is at: {url} </p>
      <button disabled = {btnState}>button</button>
<EmotionCss />
  </section>
  
  
  
  <style>
    img { width: 20em;}
  </style>
  