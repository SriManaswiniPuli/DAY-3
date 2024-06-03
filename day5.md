## SOFTWARE DEVELOPMENT LIFE CYCLE
- 1.Planning -Planned by CEO
- 2.Analysis -2types-Business,Technical
- 3.Design -(Sketch)Designers use Figma Vscode,Adobe Xd;Prototyping is faster
- 4.Implementation-Implemented by Developers
- 5.Testing and Integration
- 6.Maintenance

## Stakeholders

-People who are responsible for make of a product,responsible if anything goes wrong of  a product.They are the one's who are taking risk,by holding a share of the  company.

# 6 Phases of SDLC
1. Analysis-Product Owner,Project Manager,Business Analyst,CTO
2. Design-System Architect,UX/UI Designer
   > System Archiect-People who set up the project initially(lay a foundation),set up the blueprint of the project,They need to have knoweldge of everything
3. Development-Front-end Developer.Back-end Developer
4. Testing-Solutions Architect,QA Engineer,Tester,DevOps
5. Deployment-Data Administator,Devops
6. Maintenance-Users,Testers,Support Managers

![alt text](<Screenshot 2024-06-03 112806.png>)

## Waterfall and Agile Models

![alt text](<Screenshot (3)-1.png>)

- Waterfall(step-by-step process) model takes 6 months.
- Agile follows cyclic pattern.

## SCRUM

![alt text](<Screenshot (5).png>)

> <b>Story Points</b>-The time duration assigned to complete a particular task in the scrum
> Example of waterfall in IT is change from react to angular(change in technologies)
> For waterfall,it has 2 releases whereas sprint has 12 releases
> 1 sprint is of 2 weeks
> 1 week for development
> 1 week for testing

![alt text](<Screenshot (6)-1.png>)
- Blocked PM -somewhere stuck in between

![alt text](<Screenshot (3)-2.png>)

## BURNDOWN CHART

- It describes the task flow
- ![alt text](<MicrosoftTeams-image (1).png>)

## KANBAN BOARD

- It is a tool for managing the scrum.
- Spill-over-The work which is assigned to next sprint which has not been done in previous sprint

## Coding Standards

- are meant to have uniformity throughout the code base.
1. Code quality
2. Dry
3. Variables names
      understandable/descriptive
      ```js
        let a=10;//❌
        let age=10;//✅
      ```
      camelCase
      ```js
      let student_name="manu"//w❌
      let studentName="manu"//✅
      ```
4. Errors

    1. Reserved keywords('if','for')
    ```js 
    let if="manu"//❌
    ```
    2. cannot start with numbers
    ```js
    let 2cool="manu"//❌
    ```
    3. cannot have special symbols($,@,#,!) (except for '_')

    ```js
    let abc$123="manu"//❌
    let abc_123="manu"//✅
    ```

    4. Choose 'let' over 'var';'const' over 'let'

    ```js
    let panCard="PQ00208N"//❌
    const panCard="PQ00208N"//✅
    ```

    5.write your const case

    ```js 
    const pivalue=3.14//❌
    const PI_VALUE=3.14//✅
    ```

    ## Documentation

    1. Single comment-//
    2.Multiple comment-
        ```js
        /**
         *This is
         * a
         * cool function
         */
        ```  
-------------------------------------------
    // Write a function to make it uppercase
```js
/**
 * Multiplies two numbers.
 * @param {number} x - The first number.
 * @param {number} y - The second number.
 * @returns {number} The product of x and y.
 * @example
 * multiply(2, 3); // returns 6
 */
function multiply(x, y) {
  return x * y;
}
```
 
---------------------------------------
// Write a function to make it uppercase
```js
/**
 * Multiplies two numbers.
 * @param {str}  - The string.
 * @returns {str} The uppercase of the string.
 * @example
 * uppercase("manu"); // returns "MANU"
 */
function uppercase(str){
  return str.toUpperCase();
}
```

