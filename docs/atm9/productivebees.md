---
title: Productive Bees
description: ATM9 Productive Bees Guide
authors:
 - Jonh09 (Original Author)
 - ArcTrooper (Editor)
---

# Productive Bees

## Kaimonick's Bee Guides

[Click here to view Kai's bee guide!](../guides/kaimonickguides.md/#productive-bees)

## Jonh09's Bee Guide

Hi, I'm Jonh09 and this guide is to help people who are getting into **Productive Bees** or want to know more advanced stuff. These guides are based on ATM9 / 1.20 Minecraft. Older/newer versions may have slight differences.

If you're starting out and want to learn more, check out [Kai's Guides](#kaimonicks-bee-guides) for resumed set of guides. [Pilpoh](https://www.youtube.com/watch?v=7wg3UQ_AsAA) also has 2 video guides on bees! Also, read the **Productive Bees book** ingame; it has all you need to know, including upgrades and how they work, different types of bees, different machines, etc. A glance at the book will help if you get stuck. Also, remember that **JEI** (the item visualizer) is your best friend.

- This guide is divided in 7 parts:
	* What is **Productive Bees**, and how to start;
	* Upgrades;
	* All the machines / blocks;
	* Automation;
	* Genes/Traits
	* Complicated or otherwise hard to get bees;
	* Tips or personal advices;
	* The **WannaBee** + **Amber Bee**: ^^The Mob Farm duo^^;

If you find any errors or something that can be done differently, you can ping me in our discord, @jonh09.

Original guide: [Productive Bees GUIDE - Beginning Tutorials + Best Genes and how to get them](https://imgur.com/a/bh2fHtf)

---

### Genes

![A bee's genes](img/pb_genes.png){align=right width='249px' height='132px'}

Genes (or Traits) are the stats/attributes that bees have that determine their productivity, what conditions they can work in, and other less important ones. In this category, i will show you the best genes and how to get them.

[](){#gene_types}
---
| Gene | Description | Levels | Best Level |
| ---- | ----------- | ------ | ---------- |
| **Productivity** | Produces more combs per trip | Normal, Medium, High, Very High | Very High
| **Weather Tolerance** | Determines which weather conditions a bee can work in | [None]("Only works during Clear weather"), [Rain]("Works during Clear weather, or while it's Raining") [Any]("Works during Any weather, be it rain, or storm") | Any
| **Behavior** | What time of day the bee can work | [Diurnal]("Only work during daytime"), [Nocturnal]("Only works at night"), [Metaturnal]("Works 24/7") | Metaturnal
| **Endurance** | Affects the bee's max health | Weak, Normal, Medium, Strong | Strong
| **Temper** | Affects bee's hostility | Passive, Normal, Aggressive, Hostile | Passive

Apart from the 5 main genes, there is a 6th gene, the **bee-specific gene**. These are used to make spawn eggs of that bee. Most major mods use bee spawn eggs to connect themselves to Productive Bees. *(EX: Mystical Agriculture essence bees)*

### How to Get Genes

Now that you know what the genes are, you need to know how to get the genes. When you **squash** a bee to get genes, you will get all of its 6 different genes. The bad news? You only get a small percentage of the gene. The percentage dictates the chance that another bee has to get that gene. 

To give genes/traits to a different bee, combine a **Honey Treat** with your chosen gene(s) in a crafting grid and then `right click` a bee to give it that trait or set of traits.
*You can combine multiple Genes with a Treat, instead of making a Treat per different gene*

![Bee squashing diagram](img/pb_howtogetgenes.jpeg){.center width='500px' height='500px'}

???+ abstract "Getting genes is a pretty simple process:"
	1. Get a bee you wish to get the genes of
	2. In a 3 block tall space, put a **Bottler** *(with bottles of course)* on the bottom, and a **Piston** (facing down) on top with button/lever on a block next to it.
	3. Put the bee in the middle, and quickly press the lever/button, that will squish the bee into a bottler and give you **Squashed Bee Material**
	4. Put that into a **Centrifuge**, and it will give you the 6 genes of the bee. 

Easy right? But remember, it will only give up to around 20% of the gene per bee, so you need to repeat the process 5-6 times. I'll show you how to get genes automatically below.

---

### Gene Automation

This is a simple semi-automated setup. I reckon you already know how to set up breeding and incubation to get more bees if you are here.

![Example gene automation setup](img/pb_geneautomation.png)

#### **1.** The Dispensing of Bees

For this you can just use a vanilla **Dispenser** + an **RFTools Timer** to send a pulse to it every **20 ticks**, releasing a bee from a cage into the piston area. The lever behind the Timer is just to disable it when you arent using it.

???+ tip
	Make sure you are squishing bees in disposable cages, as those dont cause any clutter and are more straightforward to use

#### **2.** The Squishing

This is where the bees will be turned into the **Squashed Bee Material**, the same thing as in the previous explanation. Dont forget to send bottles to the **Bottler** or it will stop squishing bees.

???+ tip
	If you keep the piston extended, like in the image, the bees will get squashed automatically when you push/dispense them into it.

#### **3.** Processing Bee Material

Using any Item Collector, pick up the **Squashed Bee Material** and send it to a **Centrifuge** that separates it into the 6 genes.

#### **4.** Sorting & Improving Genes.

After getting the genes out of the centrifuge using whatever pipe you prefer, you can send them into a **Gene Indexer**. This machine will sort and combine the genes inside when given a redstone signal *(Lever or Redstone Block)*. It will combine all the genes into their 100% version. These are the ones we are looking for, the ones that allow you to change the genes of a bee 100% of the time.

#### Extra info for Sorting

Using a pipe / mod that has good filtering, you can do some neat filtering to organize your genes. 

- Examples of mods that can do that: 
	* **LaserIO**
	* **Integrated Dynamics**
	* **Pipez**

Item ID: `productivebees:gene`

- NBT filters: 
	* `{productivebees_gene_purity:100}` - for the gene percentage, this targets 100% genes;
	* `{productivebees_gene_attribute:"productivity}` - for the gene type, valid types being: `productivity`,`weather_tolerance`, `behavior`, `endurance` and `temper`;
	* `{productivebees_gene_value:0}` - for the gene level, 0 = lowest level, and biggest = highest level, this depends on the gene type. 
	<br>An example: Productivity: Normal = gene_value:0, and Productivity: Very High = gene_value:3, use the table at [Gene Types](#gene_types) to see the levels.


---

### Getting the Best Genes

OK, OK, you already know what genes are, how to get them, and how to automate them. This is what you are here for, the ***BEST*** genes. In this section, I'll discuss the most and least important ones.

???+ note 
	My recommendation? Put all your good genes into one bee that you can breed. Then, you will get a baby with the same genes.
	
	From there, breed them -> Squish them -> Get genes -> Make Honey Treats with those genes, and use those to upgrade all your bees.

???+ tip
	You can put **multiple genes** into the same **Honey Treat**. I like to call this *Bee Steroids*, a honey treat with all the best genes.

<br/>

#### ^^Least Important^^

The least important ones are **Temper** and **Endurance**. These two are worthless if you use a **Simulator Upgrade** or have them in a box.

<br/>

#### ^^Most Important^^

[]()
##### Productivity: Very High

![](img/pb_kamikaze.png){align=right, #helmet}

This one's the trickiest and most important; this trait can only be gotten from **Kamikaze Bees**.

**Kamikaze Bees** spawn in a very particular way. Their only objective is to protect you by... well... going kamikaze on the attacker.

While wearing a **Bee Nest Helmet** (a Diamond helmet with a Nest on top), if you get hit by a hostile mob, there is a **30% chance** of a Kamikaze Bee spawning. The difficult part? They're *TINY* and *FAST* so you need to have a setup inside an enclosed box using a **Catcher** with Cages inside and maybe a range upgrade, or have good aim and cage them once they spawn.

Get **5-6** of them then squeeze them. This should get you a **100% Very High** Productivity gene.

!!! warning "Kamikaze Bees can't breed with each other."

With that done now you need to put the gene you got from Squishing it in an breedable bee (*like a Iron Bee per example*) (via Honey Treat + Gene) and breed them, and once an Child bee is born with the Very High gene, *grow it* and use it to breed more bees of that type. With that, you basically have infinite, Very High Productivity genes.

<br/><br/>

##### Behavior: Metaturnal

To get this trait, a bee needs to be **left outside** leashed to a fence for a few days. <br/>*Note that the bees you choose need to be breedable, so you can use 1 with the trait to get more by breeding.

!!! info
	- How it works? Every few minutes a check for the leashed bee is done, and on that check, 4 things can happen:
		* **^^During the Day^^**: 90% chance for Nocturnal -> Metaturnal ***or if you are unlucky*** 10% chance for Nocturnal -> Diurnal
		* **^^During the Night^^**: 85% chance for Diurnal -> Nocturnal ***or if you are lucky*** 15% chance for Diurnal -> Metaturnal
		* ^^Every time a check fails, the bee will **take damage**. Make sure to feed the bees with **Honey Treat** to heal them.^^
I usually have like 10 bees leashed, and if im lucky enough, after like half an hour i should have a couple of metaturnals in there.

<figure markdown="span">
  ![Image title](img/pb_behavior.png){ width='350px' height='350px' }
</figure>

<br/><br/>

##### Weather Tolerance: Any

There are 2 ways to obtain this. The slow and the fast way. 

The slow: The strategy of leaving the bees outside so they get forced to adapt like the previous one... OR the fast fishing route. 

By fishing I mean fishing for bees, more specifically either **Prismarine Bees** or **Water Bees**. <br>

- Differences and where to find:
	* **Prismarine Bee** comes with ^^**Any**^^ Weather Tolerance, and ^^**Strong**^^ Endurance -> Can be found in any `Deep Ocean` biome;
	* **Water Bee** comes with ^^**Any**^^ Weather Tolerance -> Can be found in `River` biome.

You will need 2 of those to breed them to make more and to get that sweet weather tolerance. 
!!! tip 
	Technically you only need one bee, as there is a neat trick you can do to make a bee breed with itself.
	<br>Get a **Advanced Hive** + **Expansion Box**, use either 1 **Simulator** and 3 **BaBee** upgrades, or 4 **BaBee** upgrades.
	<br>One cool thing the **BaBee Upgrade** does, is that it can make bees in a hive breed naturally, and only 1 bee is needed, not 2 like normal breeding. 
	<br>(*This does not work for bees that can't breed between themselves*)

???+ note 
	When a bee gets fished out, it will get **angry**, the best way to prevent getting attacked by it, and prevent the bee from dying is:
		<br>**Wear a Bee Nest Helmet** - the same mentioned in the [Productivity](#helmet) chapter, as the tooltip says, "Angry bees won't attack you".
		<br>**Use a Catcher** with some range upgrades - it will catch the bee if its in range.

 
!!! tip "If there aren't deep oceans or rivers nearby, use a **Nature's Compass** to point you to a river."

![](img/pb_prism_water_bees.png){.center height='250px'}


### Genes When Breeding

When breeding, you must know how genes are assigned to a child bee.

The bee on the **Left** side will be the **Main** bee, which is the one with priority gene-wise. This means that the baby will have the genes of the main bee as base, never lower. 

The bee on the **Right** only defines the range/max level of genes.

In the image below the "maxed" gene levels of the **Main** bee (Weather tolerance, behavior, and endurance) gets transferred to the child bee.

![](img/pb_breedingpair.png){.center}

???+ example
	If the main bee has **Productivity: Medium**, and the 2nd bee has **Productivity: Very High**, the baby will have a chance to have either Medium (the minimum the main bee has), High, or Very High.

You will *never* get a child bee that has genes of a lower level than the main bee. That's why I recommend maxing out the 1st bee so it can be used as the main one for breeding.

> Productive Bees | [CurseForge](https://legacy.curseforge.com/minecraft/mc-mods/productivebees)
