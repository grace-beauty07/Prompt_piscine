# Objective: Create a reusable prompt for text summarization.
-----
## Weak prompt 1: "Summarize this text." (a short article about art)
## Output:
>### The article argues that art is not some decorative hobby humans invented to feel cultured. It is a fundamental part of being human. From ancient cave paintings to children drawing with crayons, art helps people interpret the world and express emotions that words often fail to capture. It supports emotional intelligence, mental health, and self-understanding by creating a space where inner experiences can be explored safely.
>### It emphasizes the importance of art education, especially for young people. Teachers describe art classrooms as low-pressure environments where students explore identity, race, environmental issues, and personal interests. Through art, students gain a “visual language” to process complex topics and develop empathy and confidence.
>### The article also highlights community-based art education at Colorado State University. Programs like BRAINY and Family Day, hosted at the Gregory Allicar Museum of Art, connect university students with K–12 learners, especially those from underserved communities. These programs aim to make art accessible, promote inclusion, and strengthen community bonds. The broader claim is that art contributes to responsible citizenship, social awareness, and healthier communities overall.
>### In short: art is framed as emotionally vital, socially connective, and educationally transformative. Not just “nice to have,” but essential to human development and community wellbeing.
-----
## Refined prompt 1: "Summarize the above text in 3 bullet points, focusing on the main arguments and ignoring examples."
## Output:
>- ### Art is a fundamental part of human nature, essential for emotional expression, self-understanding, and interpreting the world.
>- ### Art education supports personal growth, empathy, identity development, and social awareness.
>- ### Art strengthens communities and contributes to responsible citizenship and overall societal wellbeing.
-----
## Weak prompt 2: "Summarize this text." (a technical blog)
## Output:
>### The article argues that strong API documentation is essential for successful integration and developer adoption. It lays out 11 key components, starting with clear “Getting Started” instructions that explain authentication, API keys, and first calls so developers can begin quickly and confidently.
>### It emphasizes practical, developer-friendly features such as interactive examples, executable collections, code snippets in multiple languages, and a comprehensive endpoint catalog. These elements reduce friction, speed up learning, and make APIs accessible to a broader range of developers.
>### The guide also stresses security details, rate limiting information, troubleshooting support, sandbox environments, and community engagement. Together, these build trust, improve resilience, and create a sustainable ecosystem around the API rather than just a technical reference document.
>### In short: great API documentation is not a static manual. It is an interactive, secure, developer-centered experience that supports learning, scaling, and community growth. Which, frankly, is what separates usable APIs from the digital equivalent of a locked door with no key.
-----
## Refined prompt 2: "Summarize the above text in 3 bullet points, focusing on the main arguments and ignoring examples."
## Output:
>- ### High-quality API documentation is critical for successful developer adoption and effective API use.
>- ### Documentation should be clear, structured, and developer-focused to reduce friction and improve usability.
>- ### Strong documentation builds trust, supports scalability, and fosters a sustainable developer ecosystem.
-----
## Testings with two different inputs:
>- ### Link to art article - https://magazine.libarts.colostate.edu/article/art-is-an-essential-part-of-the-human-experience/
>- ### Link to technical blog - https://blog.postman.com/2024-guide-to-mastering-api-documentation/
