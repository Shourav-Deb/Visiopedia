
---

<h1 align="center">🥽 Visiopedia: A Comparative Performance Study 🥽</h1>
<p align="center">
  <i>Exploring How Machines Learn Visual Concepts Without Labels</i>
</p>


<p align="center">
  <img src="https://i.pinimg.com/736x/e7/4b/ce/e74bcea049a8eb1d5c2df7c6131a2d3b.jpg" alt="Web Development Showcase Banner" width="1200">
</p>



## ✨ What is Visiopedia?

**Visiopedia** is an interactive visual concept explorer that demonstrates how machines can **learn and reason about images without explicit labels**.

Instead of predicting class names like a traditional classifier, Visiopedia:
- Learns **visual concepts** from a small set of example images
- Builds **self-supervised visual prototypes**
- Explains what it “sees” in new images using **visual similarity**, not predictions

> 💡 In short: **Visiopedia shows how machines understand images by comparing them to previously seen visual examples.**

---

## 🔬 Background: The Betel Leaf SSL Project

Visiopedia is built on top of a larger academic mini-project focused on **Self-Supervised Learning (SSL)** using the **[Betel Leaf dataset](https://data.mendeley.com/datasets/btdym2t6mt/1)**.

In the original project, I conducted a complete, research-oriented study that included:

- Exploratory Data Analysis (EDA) on the Betel Leaf dataset  
- Supervised baselines using pretrained CNN architectures  
- Self-Supervised Learning using **SimSiam**  
- Label-free pretraining and downstream evaluation  
- Linear probing, k-NN evaluation, and full fine-tuning  
- Embedding analysis using PCA, t-SNE, and UMAP  
- Label-efficiency studies and ablation experiments  

The **SimSiam encoder trained during this project** is the core visual representation model used in Visiopedia.

> 📄 **For full academic details, experiments, and works, please refer to the [Project Description](https://github.com/Shourav-Deb/Visiopedia/blob/main/Project%20Description.pdf) PDF included in this repository.
> For Training Notebook or Model you can [contact](mailto:heyneeddev@gmail.com) anytime.**

## 🧠 From Research to Visiopedia

After completing the Betel Leaf SSL project, I extended the work into **Visiopedia** to make the learned representations:

- Interactive  
- Explainable  
- Usable beyond a single dataset  

Visiopedia transforms the trained SSL encoder into a **concept-learning and reasoning system**, allowing users to *teach*, *test*, and *explore* visual understanding directly in a web interface.

---

## 🚀 What Visiopedia Does

### ✅ Teaching Phase (No Labels Required)
- Upload **at least 3 images of the same object** [More Picture More Detailed Learn]
- Assign a human-readable name [The name is not learned, It is only used to describe similarity results]
- Visiopedia builds a **visual prototype** using self-supervised embeddings


### 🔍 Testing Phase (Similarity-Based Reasoning)
When a new image is uploaded, Visiopedia:
- Compares it against all learned visual prototypes
- Measures **relative similarity in embedding space**
- Explains results using natural language, such as:
  - *“I can clearly see this object”*
  - *“I might also see this one, but I’m not confident”*
  - *“I don’t see any trace of this object”*

- Multiple objects can be detected **simultaneously** if they are visually present.
- Visiopedia itself is **dataset-agnostic** and can be used with any images


## 🌐 How to Use Visiopedia

Visiopedia works in two simple stages: **Teach** and **Explore**.  
You do not train a classifier. Instead, you teach the system **visual concepts** and observe how it reasons using **visual similarity**.



### 🔹 Step 1: Teach Visual Objects

Navigate to **Step 1: Teach Visual Objects**.

For each visual object:

1. Upload **at least 3 images** of the same object  
2. Enter a **name** for the object  
   - This name is for your reference only  
3. Click **Save Object**

Repeat this process to add more objects.

#### Key Details
- You can add **up to 5 visual objects**
- Saved objects appear in the **Learned Objects gallery**
- The system does **not** learn the name  
- It learns the **shared visual pattern** across the uploaded images



### 🔹 Step 2: Lock the Knowledge

Once you finish teaching:

1. Click **Lock & Start Testing**

This action:

- Freezes all learned objects
- Prevents further edits during testing
- Ensures **fair and consistent comparison**

You can **unlock** the system at any time if you need to modify or add objects.



### 🔹 Step 3: Explore New Images

After Lock It Will Go to **Step 2: Test Images**.

1. Upload one or more new images

For each image, Visiopedia will:

- Compare it against **all learned visual objects**
- Display **relative similarity bars**
- Generate a **natural language explanation** describing what it perceives, such as:
  - Clearly visible objects
  - Possibly present objects
  - Weak or uncertain traces
  - No recognized objects

Multiple objects can be detected in a single image if sufficient visual similarity exists.



### 🔹 Understanding the Output

- Confidence bars represent **relative similarity**, not probability
- Higher bars indicate **stronger visual resemblance**
- The explanation text summarizes what the model “sees”

### Important Clarifications
- Visiopedia does **not** classify
- It does **not** predict labels
- All reasoning is based purely on **visual similarity in embedding space**



### 🔹 Editing or Resetting

You can **unlock** the system at any time to:

- Delete existing objects
- Add new objects
- Teach different visual concepts

After making changes, **lock** the system again to resume testing.



### ⚠️ Important Notes

- Results depend on **visual similarity**, not semantic correctness
- The system may detect **multiple objects** in one image
- If no learned object matches, Visiopedia will explicitly state that nothing was recognized

---

## ✨ Key Features

- 🧠 Self-supervised visual representation learning (SimSiam)
- 🏷️ No label-based classification
- 📦 Prototype-based concept memory (up to 5 objects)
- 🔐 Lock / Unlock workflow to prevent accidental edits
- 📊 Confidence bars for each learned object
- 🗑️ Object management (add / delete concepts)
- 🌐 Interactive **Streamlit web app**
- 🎨 Premium, Friendly UI



## 🛠️ Tech Stack

- **Python**
- **PyTorch**
- **SimSiam (Self-Supervised Learning)**
- **NumPy**
- **Streamlit**
- **PIL**

Training and experimentation were conducted using **Kaggle / Colab environments**, while Visiopedia is designed as a lightweight interactive deployment.



**🎉 Happy exploring visual reasoning with Visiopedia. Hope you like it. 🎉**
---
