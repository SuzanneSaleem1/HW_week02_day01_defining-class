# Kotlin I Assignment  I defining class
---
The Kotlin assignment has one component:
- writing code(required)
- open-ended question (optional)
- ...
> Note: You must save your solution as `homeworkSolution.kt`.

## Part I - defining a class ( writing code "required").
---
###  `write a kotlin program with student class that has three proprty "name" and "age" and "GPA"` 
### ` and give the student  abilty to (speake hint:use print ) and the abilty to add two numbers `
###
## Part II - open-ended question ( optional ) .
---
### read the code below and answer the questions
### 
> ### class Weapon(val name: String)
>  ##### class Player {
> ##### var weapon: Weapon? = Weapon("Ebony Kris")
> ##### fun printWeaponName() {
> ##### if (weapon != null) {
> ##### println(weapon.name)
> ##### }
> ##### } }
> ##### fun main() {
> ##### Player().printWeaponName()
> ##### }

### Q1 = what dose Race Conditions mean
race condition occurs when two (or more) threads are operating on the same data at the same time, 
meaning a thread could end up using stale data
###
### Q2 = is there any Race Conditions in the code
###
 yes, becuase there is a possibility  of weapon being null betweeen the time check passesd and and the time the name is printed. the compiler balks becouse it cannot
###
### Q3 = what's the best way to solve the compiling error in the code using scopeFunction
fun printWeaponName() {
weapon?.also{
println(it.name)}}
###
###
