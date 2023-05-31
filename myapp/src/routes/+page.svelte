    <script>
       
        let mousePosition ={ x: 0 , y: 0};

        function mouseTrack(event){
            mousePosition.x =event.clientX - 10;
            mousePosition.y =event.clientY - 10;
            
        }
        
    </script>
  
  
  
  <div>

    

    
    <div  class="inner-ground" on:mousemove={mouseTrack}> 
        <canvas id="battle-ground" class="battle-ground"   >
         </canvas>
        
    </div>
    

    <button class="button-1"></button>
    <button></button>
    <button></button>

    <p>mouse position is x: {mousePosition.x} y: {mousePosition.y}</p>


  </div>
  
  <style>
    .battle-ground{
        border: 3px solid black;
        display:  inline-block;
        height:100% ;
        width: 100%;
        background-color: lightgreen;
        position: absolute;
       
    }
    .inner-ground{
        width: 300px;
        height: 300px;
        position: relative;
         
    }
    
    
  </style>