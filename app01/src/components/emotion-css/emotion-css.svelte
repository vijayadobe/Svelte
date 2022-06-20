<script>
    import { css } from '@emotion/css'
     
      
        const ORANGE = "#ffa500";
        const RED = "red";
        const WHITE = "white";
        const wide = "30em";
      
        // needs to be configured using variables.
        const heading = css`
          background-color: ${ORANGE};
          color: ${WHITE};
          width: ${wide} ;
        `;
      
        const Button = css`
          border: none;
          color: white;
          padding: 14px 28px;
          cursor: pointer;
          background-color: ${ORANGE};
          &:hover {
            background-color: ${RED};
          }
        `;
        
      </script>
    
      
      <div>
        <h5 class={heading}>This style is from CSS-in-JS</h5>
        <button class={Button}>Hover on this block...</button>
      </div>
    
    