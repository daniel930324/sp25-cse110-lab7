Name: Huei-Guo Chang

Check Your Understanding questions
1. Where would you fit your automated tests in your Recipe project development pipeline? Select one of the following and explain why.
    - Answer: 1. Within a Github action that runs whenever code is pushed.
    - Because all other options just doesn't look right and we just learned about Github action that meets the requirement in the question.
    - Although I think it would be great to be able to manually run test locally and not have to only test them when trying to push, I think this is just not the requirement of "automated" tests the question is asking
    - Run the tests all after all development is just going to be a mess if there exists bugs in the code.

2. Would you use an end to end test to check if a function is returning the correct output? (yes/no)
    - No, I think unit test is the one that do this job

3. What is the difference between navigation and snapshot mode?
    - Navigation mode reloads the site from scratch and measures real‑world load performance.
    - Snapshot mode examines the page as it is right now, focusing on static audits like accessibility, best‑practices, and SEO, but without simulating a full page load or recording interactions.
   
4. Name three things we could do to improve the CSE 110 shop site based on the Lighthouse results.
    - Add a mobile viewport tag
      - The site is missing <meta name="viewport" content="width=device-width, initial-scale=1">, which hurts mobile rendering and adds a 300 ms tap delay
    - Speed up the Speed Index
      - An 8.0 s Speed Index is failing—minify/ defer render‑blocking JS & CSS or compress images to get that under 2 s 
    - Let returning visitors load instantly
      - By telling the browser to keep icons, scripts, and other files around for longer, repeat visitors won’t have to re‑download them. That way, the pages pop up almost instantly on their next visit