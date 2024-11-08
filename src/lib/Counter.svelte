<script>

  let count = 0
  
  const increment = () => {
  
  if(count<20){
    count +=1
  }
  }
  const decrement = () => {
    if(count>0){
      count -=1
    }
  }
  
  </script>
   <h1>{count}</h1>
   <button id="+" onclick="{increment}">+</button>
   <button id="-" onclick="{decrement}">-</button>
  