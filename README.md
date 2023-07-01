# CSS Grid (The ultimate layout tool)

    > Flexbox was our first layout tool in CSS.
      - It's amazing. We can do fantastic things with it, and it's super great at being flexible, but it has its limitations.

      - Flexbox only deals with 1-dimension at a time.
        - If we have "flex-direction: row;" we get columns. (We are working on the horizontal dimension)
        - If we have "flex-direction: columns;" , we get row. (We are working on the vertical dimension)

    > What if we want rows & columns?
        - We can use CSS Grid.

        - CSS Grid enables us to create grid, that means we can work on both vertical and horizontal axis at the same time!
        - This opens up new layout possibilities that we simply didn't have before.
        - It also enables us to simplify our markup.
        - It's great because we don't have to think so hard about how content need to be grouped, resulting in much "flatter" HTML.

    > It does come with some added complexity too.
    
      - The ultimate layout tool:
        -  grid-template-columns: ;
        - grid-template-rows: ;
        - grid-auto-columns: ;
        - grid-auto-rows: ;
        - grid-column-start: ;
        - grid-column-end: ;
        - grid-row-start: ;
        - grid-row-end: ;
        - grid-template-areas: ;
        - grid-gap: ;
        - minmax();
        - repeat();
        - fr
        and many more.


## Setting up a grid:

  > The first step to creating a grid is declairing "display:grid;" on the parent element.

  > This creates a new grid formatting context. This is similar to when we declare "display: flex;" in many ways.

  > Margin no longer collapse and the direct children of the element become grid items.

  > Similar to flexbox, when we create a new grid container, the flex children will fall onto the grid.

  > The only real change we'll see at first though, is that the margins no longer collapse. We have no dramatic making columns like if we created a flex container.

  
### To properly use CSS grid we need to define rows and columns.

  - Because flexbox only deals with one dimension, we don't have to worry about rows and columns,we can just swithch back and forth with flex-direction.
  - With grid, we have both. We can explicitly create them and then place items within the grid that we have created.

    - We do that with "template rows and columns" :-

      Ex: 
          grid-template-columns: 200px 200px 350px;

          grid-template-rows: 50px 200px;

        Ex: 
            body {
                display: grid;
                grid-template-columns: 300px 100px 100px 200px;
                grid-template-rows: 750px 500px
            }


            *- Short-hand for grid-template:

              Ex:
                  body {
                      display: grid;
                      grid-template: 100px 400px / 250px 250px 250px;
                  }

                  (grid-template: rows / columns;)

    ### Placing items on the grid:

      > Content will place itself automatically on the grid.
      
      > We can explicitly place items where we want them to be.

      > We can tell grid items exactly where they live within their parent's grid with the following properties:

          - grid-column-start
          - grid-column-end
          - grid-row-start
          - grid-row-end

          



