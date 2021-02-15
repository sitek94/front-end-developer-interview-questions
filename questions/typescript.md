# TypeScript

<details>
  <summary>What's the difference between type `any` and `unknown`?</summary>

  * `unknown`
    * type of variable that we do not know when we're writing an app
    * these values may come from dynamic content - e.g. from the user
    * we can narrow it down to something more specific by doing `typeof` checks,
      comparison checks or more advanced type guards
      ```ts
      declare const maybe: unknown;

      if (typeof maybe === 'string') {
        console.log(maybe.toUpperCase());
      }
      ```
  * `any`
    * powerful tool to work with existing JavaScript, so we can gradually opt-in and opt-out of type
      checking
    * when not all type information is available or its declaration would take a lot of effort, this
      might happen for values from code that has been written without TypeScript or a 3rd party library
    * unlike `unknown` variables of type `any` allow us to access aribtrary properties, even
      ones that don't exist
      ```ts
      let anyVar: any;
      let unknownVar: unknown;

      console.log(anyVar.someProp);
      console.log(unknownVar.someProp); // Error: Object is of type `unknown`
      ```
</details>