# Objective: Create prompts that produce structured machine-readable output.
-----
# Unstructured information prompt:
>## List the seven wonders of the world and their locations
## Model output:
Humanity really looked at giant rocks and said, “Yes. This. This will impress people for thousands of years.” And honestly… it worked. 😌

Here are the **New Seven Wonders of the World (2007 list)** and where they’re located:

---

### 1. Great Wall of China

![Image](https://www.airpano.com/files/china_wall_01_big.jpg)

![Image](https://media.sciencephoto.com/f0/38/80/62/f0388062-800px-wm.jpg)

![Image](https://www.worldhistory.org/uploads/images/4582.jpg)

![Image](https://images.chinahighlights.com/allpicture/2014/07/a75e71599fcc40d1b72fb2b8_cut_800x500_61.jpg)

📍 Location: China
A massive ancient defensive wall stretching over 13,000 miles. Because apparently “keep out” signs were not dramatic enough.

---

### 2. Petra

![Image](https://upload.wikimedia.org/wikipedia/commons/2/2f/Treasury_petra_crop.jpeg)

![Image](https://media.assettype.com/outlooktraveller%2Fimport%2Fpublic%2Fuploads%2Ffilemanager%2Fimages%2FAd-Deir-monastery-in-Petra.jpg?auto=format%2Ccompress\&w=640)

![Image](https://upload.wikimedia.org/wikipedia/commons/thumb/2/2f/Treasury_petra_crop.jpeg/250px-Treasury_petra_crop.jpeg)

![Image](https://res.cloudinary.com/ddjuftfy2/image/upload/f_webp%2Cc_fill%2Cq_auto/memphis/large/724259958_15104168252_3f12754438_c%20%281%29.jpg)

📍 Location: Ma'an, Jordan
A stunning city carved into pink sandstone cliffs. Imagine carving an entire city out of rock without modern tools. Casual.

---

### 3. Christ the Redeemer

![Image](https://upload.wikimedia.org/wikipedia/commons/4/4f/Christ_the_Redeemer_-_Cristo_Redentor.jpg)

![Image](https://upload.wikimedia.org/wikipedia/commons/thumb/e/e7/Aerial_view_of_the_Statue_of_Christ_the_Redeemer.jpg/330px-Aerial_view_of_the_Statue_of_Christ_the_Redeemer.jpg)

![Image](https://cdn.cnn.com/cnnnext/dam/assets/170305125355-christ-the-redeemer-rio-vr-full-169.jpg)

![Image](https://s.abcnews.com/images/US/ABC_christ_redeemer_jef_140713_16x9_992.jpg?w=384)

📍 Location: Rio de Janeiro, Brazil
A 98-foot statue overlooking the city. Calm, iconic, slightly judging all of us.

---

### 4. Machu Picchu

![Image](https://cdn.mos.cms.futurecdn.net/WFJBpzs4J5x3uvbeKdnm3i.jpg)

![Image](https://images.squarespace-cdn.com/content/v1/596b2969d2b85786e6892853/7d85da8b-7093-4276-9591-9074b8c2b5a8/0K3A3715.jpg)

![Image](https://iblog.iup.edu/trowelsandtribulations/files/2022/11/Agricultural-Terraces.png)

![Image](https://www.amautaspanish.com/fotos/galeria/big/terraces-built-at-machu-picchu-site.jpg)

📍 Location: Cusco Region, Peru
An ancient Incan city high in the Andes. Built on a mountain because flat land is clearly overrated.

---

### 5. Chichen Itza

![Image](https://upload.wikimedia.org/wikipedia/commons/5/51/Chichen_Itza_3.jpg)

![Image](https://www.chichenitza.com/public/assets/img/ruins/el-castillo-chichen-itza.jpg)

![Image](https://maya.nmai.si.edu/sites/default/files/null/chichenitza_s1.jpg)

![Image](https://upload.wikimedia.org/wikipedia/commons/d/df/Chichen_Itza_Mexico_%28125162457%29.jpeg)

📍 Location: Yucatán, Mexico
A massive Mayan pyramid complex. Architecture plus astronomy plus mystery equals legend.

---

### 6. Roman Colosseum

![Image](https://upload.wikimedia.org/wikipedia/commons/thumb/d/de/Colosseo_2020.jpg/1280px-Colosseo_2020.jpg)

![Image](https://www.walksinsiderome.com/_next/image/?q=75\&url=https%3A%2F%2Fwww.walksinsiderome.com%2Fuploads%2F2024%2F09%2FIMG_20240515_113357-scaled.jpg\&w=1920)

![Image](https://dynamic-media-cdn.tripadvisor.com/media/photo-o/2f/1f/c1/34/caption.jpg?chk=v1_19b8fd93573cc10705fb\&cx=1920\&cy=1080\&h=-1\&s=1\&w=1200)

![Image](https://www.walksinsiderome.com/uploads/2020/04/colosseum-at-night.jpg)

📍 Location: Rome, Italy
An enormous amphitheater where gladiators once fought. Humanity has always loved spectacle. Some things never change.

---

### 7. Taj Mahal

![Image](https://media-cdn.tripadvisor.com/media/attractions-splice-spp-674x446/06/70/65/83.jpg)

![Image](https://upload.wikimedia.org/wikipedia/commons/4/4d/TajMahalbyAmalMongia.jpg)

![Image](https://upload.wikimedia.org/wikipedia/commons/b/bd/Taj_Mahal%2C_Agra%2C_India_edit3.jpg)

![Image](https://media.architecturaldigest.com/photos/67acb9b0339bcbaaadeb91b5/1%3A1/w_4000%2Ch_4000%2Cc_limit/GettyImages-873536102.jpg)

📍 Location: Agra, India
A breathtaking white marble mausoleum built as a symbol of love. Dramatic romantic energy. 💔🤍

---
 
There you go. Seven reminders that when humans focus their energy on beauty instead of chaos, they can actually do incredible things. Kind of hopeful, if you think about it.

---

## Rewritten prompt
>## List the seven wonders of the world and their locations. Return the following in JSON format: [{wonders of the world: string, location: string}].
## Model output:
```json
[
  {
    "wonders of the world": "Great Wall of China",
    "location": "China"
  },
  {
    "wonders of the world": "Petra",
    "location": "Ma'an, Jordan"
  },
  {
    "wonders of the world": "Christ the Redeemer",
    "location": "Rio de Janeiro, Brazil"
  },
  {
    "wonders of the world": "Machu Picchu",
    "location": "Cusco Region, Peru"
  },
  {
    "wonders of the world": "Chichen Itza",
    "location": "Yucatán, Mexico"
  },
  {
    "wonders of the world": "Roman Colosseum",
    "location": "Rome, Italy"
  },
  {
    "wonders of the world": "Taj Mahal",
    "location": "Agra, India"
  }
]
```

---

## Testing with multiple inputs:
>## Ololade Bankole, age 37, lives in Abuja and works as a Chef at Smallville Hotel Nkechi Umeh, age 65, lives in Lagos and works as a teacher at Queensland Private School Itunu Oni, age 70, lives in Paris and works as a Coding Mentor at Learn2Earn Jesus Navas, age 65, lives in Spain and works as a footballer at PSG. Return the following in JSON format: [{Name: string, Age: number, Location: string, Occupation: string, Company name: string}].
## Model output:
```json
[
  {
    "Name": "Ololade Bankole",
    "Age": 37,
    "Location": "Abuja",
    "Occupation": "Chef",
    "Company name": "Smallville Hotel"
  },
  {
    "Name": "Nkechi Umeh",
    "Age": 65,
    "Location": "Lagos",
    "Occupation": "Teacher",
    "Company name": "Queensland Private School"
  },
  {
    "Name": "Itunu Oni",
    "Age": 70,
    "Location": "Paris",
    "Occupation": "Coding Mentor",
    "Company name": "Learn2Earn"
  },
  {
    "Name": "Jesus Navas",
    "Age": 65,
    "Location": "Spain",
    "Occupation": "Footballer",
    "Company name": "PSG"
  }
]
```
---
## The JSON stays valid
