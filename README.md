This project was bootstrapt with [vue create app](https://cli.vuejs.org/guide/creating-a-project.html)

To run the project locally clone the repo and install project dependencies: npm install on the project root

To compile and serve the project: npm run serve

Emulates the layout of icons on a smart phone

- screen more than 1000px: show 6 columns
- 500px-999px: shows 4 columns
- below 500px: show 2 columns

- Icon should be draggable. To drag an icon a user must click and hold for a second or so. used [vuedraggable](https://github.com/SortableJS/Vue.Draggable) library
- Dragging an icon into other icons should reorder the icons on the screen.
- CSS only wallpaper design.
