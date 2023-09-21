#PARA INSTALAR UNA LIBRERIA#
Install.packages("raster")

#Para cargar una libreria#
library(raster)
#para definir el directorio de trabajo#
setwd("C:/Users/Alumno/Desktop")

getwd()
setwd("C:/Users/Alumno/Desktop")
list.files()                 
Libro2 <- read.delim("C:/Users/Alumno/Desktop/Libro2.txt")
View(Libro2)
View(Libro2)
library(readr)
Libro2 <- read_csv("Libro2.csv")
data=read.delim("Libro2.txt")
my_character="universe"
my_character
my_character
my_numeric=42
my_character="universe"
my_logical=FALSE
class(my numeric)
class(my_numeric)
class(my_character)
class(my_logical)
vegas="Go!"
=======================vectors============================================
numeric_vector=c(1,10.49)
character_vector=c("a","b","C")
boolean_vector=c(TRUE,FALSE,TRUE)
poker_vector=c(140,-50,20,-120,240)
roulette_vector=c(-24,-50,100,-350,10)
names(poker_vector)=c("Monday","Tuesday","Wednesday","Thursday","Friday")
poker_vector
days_vector=c("lunes","martes","miercoles","jueves","viernes")
names(poker_vector)=days_vector
names(poker_vector)=days_vector
poker_vector
names(roulette_vector)=days_vector
roulette_vector
total_daily=poker_vector+roulette_vector
roulette_vector
total_daily
total_poker=sum(poker_vector)
total_roulette=sum(roulette_vector)
total_poker
total_week=total_roulette+total_poker
total_week
total_poker>total_roulette
toltal_poker<total_roulette
total_poker<total_roulette
total_poker>total_roulette
toltal_poker<total_roulette
total_poker<total_vector
total_poker<total_roulette
poker_wednesday=poker_vector[3]
poker_wednesday
poker_midweek=poker_vector[c(2,3,4)]
roulette_seleccion_vector=roulette_vector[2:5]
roulette_seleccion_vector
poker_start=poker_vector[c("lunes","martes","miercoles")]
poker_start
mean(poker_start)
poker_start=poker_vector[c("lunes","martes","miercoles")]
mean(poker_start)
selection_vector=poker_vector>0
selection_vector
poker_winning_days=roulette_vector[selection_vector]
poker_winning_days
======================matrix============================================
#Construct a matrix with 3 rows that contain the numbers 1 up to 9
matrix(1:9, byrow= TRUE, nrow= 3)

matrix(1:9,byrow=TRUE,nrow=3)
matrix(1:9,byrow=FALSE,nrow=3)
new_hope=c(460.998,314.4)
empire_strikes=c(290.475,247.900)
return_jedi=c(309.306,165.8)
new_hope
empire_strikes
return_jedi
box_office=c(new_hope,empire_strikes,return_jedi)
box_office
star_wars_matrix=matrix(box_office,nrow=3,byrow=TRUE)
star_wars_matrix
#Vectors region and titles, used for naming
region=c("us","non-us")
colnames(star_wars_matrix)=region
titles=c("a new hope","the empire strikes back","return of jedi")
#Name the columns with the region
colnames(star_wars_matrix)= region
#Name the rows with the titles
rownames(star_wars_matrix)=titles
star_wars_matrix
view(star_wars_matrix)
#Calculate worlwide box office figures
worldwide_vector=rowSums(star_wars_matrix)
star_wars_matrix
#Bind the new variable worldwide_vector as a column to star_wars_matrix
all_wars_matrix=cbind(star_wars_matrix,worldwide_vector)
star_wars_matrix
all_wars_matrix
worldwide_vector
all_wars_matrix2=all_wars_matrix
all_wars_matrix2
all_wars_matrix3=rbind(all_wars_matrix,all_wars_matrix2)
all_wars_matrix3

==========================

Calificaciones <- read.delim("C:/Users/Alumno/Desktop/Calificaciones.txt")
View(Calificaciones)
Calificaciones <- read.delim("C:/Users/Alumno/Desktop/Calificaciones.txt")
View(Calificaciones)
> data=read.delim("Calificaciones.txt")
> data
   alumnos calificacion
1        a            9
2        b            9
3        c            9
4        d            8
5        e            8
6        f            8
7        g           10
8        h            0
9        i            3
10       j            5
11       k           10
12       l            7
13       m            6
14       n            6
15       o           10
str(data)
'data.frame':	15 obs. of  2 variables:
 $ alumnos     : chr  "a" "b" "c" "d" ...
 $ calificacion: int  9 9 9 8 8 8 10 0 3 5 ...
data=as.data.frame(Calificaciones)
str(data)
'data.frame':	15 obs. of  2 variables:
 $ alumnos     : chr  "a" "b" "c" "d" ...
 $ calificacion: int  9 9 9 8 8 8 10 0 3 5 ...
library(ggplot2)
p=ggplot(data=df, aes(x=alumnos, y=calificacion)) + geom_bar(stat="identity")
Error in `ggplot()`:
! `data` cannot be a function.
ℹ Have you misspelled the `data` argument in `ggplot()`
Run `rlang::last_trace()` to see where the error occurred.
df
function (x, df1, df2, ncp, log = FALSE) 
{
    if (missing(ncp)) 
        .Call(C_df, x, df1, df2, log)
    else .Call(C_dnf, x, df1, df2, ncp, log)
}
bytecode: 0x000001aab79cbf20>
environment: namespace:stats>
data
   alumnos calificacion
1        a            9
2        b            9
3        c            9
4        d            8
5        e            8
6        f            8
7        g           10
8        h            0
9        i            3
10       j            5
11       k           10
12       l            7
13       m            6
14       n            6
15       o           10
str(data)
'data.frame':	15 obs. of  2 variables:
 $ alumnos     : chr  "a" "b" "c" "d" ...
 $ calificacion: int  9 9 9 8 8 8 10 0 3 5 ...
p=ggplot(data=data, aes(x=alumnos, y=calificacion)) + geom_bar(stat="identity")
p
p + coord_flip()
===================================GGPLOT====================================================
set.seed(136)
df <- data.frame(y = rnorm(300),group = sample(LETTERS[1:3],size = 300,replace = TRUE)) 
df
ggplot(df, aes(x = group, y = y)) + geom_boxplot()
box
box=ggplot(df, aes(x = group, y = y, fill = group)) + geom_boxplot()
box
box=ggplot(df, aes(x = group, y = y, fill = group)) + geom_boxplot()
> box
> box=ggplot(df, aes(x = group, y = y, fill = group)) + geom_violin()
> box
> box=ggplot(df, aes(x = group, y = y, fill = group)) + geom_boxplot()
> box+geom_violin()
> box
> box + scale_shape(8) + scale_size(2) 
> box + scale_shape(8) + scale_size=2,color="blue")
> box + scale_shape(8) + scale_size=2,color="blue"
> box=ggplot(df, aes(x = group, y = y, fill = group)) + geom_boxplot()
> box
> box + geom_violin(with=0.07)
Warning message:
In geom_violin(with = 0.07) :
  Ignoring unknown parameters: `with`
> box=ggplot(df, aes(x = group, y = y, fill = group)) + geom_violin()
> box + geom_violin(width=0.07)
> box + geom_boxplot(width=0.07)
> box + geom_boxplot(width=0.5)
> boxplot( … , medcol = "yellow", boxlty = 0, whisklty = 1, staplelwd = 4, outpch = 8, outcex = 3)
> box
> box + geom_boxplot(width=0.5)
> box + geom_boxplot(width=0.5,color="yellow",fill="black")
> box + geom_boxplot(width=0.5,((group a (color="yellow"),fill="black"))
> box + geom_boxplot(A=group"grey")


=================================Heatmap==========================================================================
data <- as.matrix(mtcars)
str(data)
heatmap(data)
data   
colcrot=c("Caquilus","Carmstrongi","Ccampbelli","Cintermedius","Cpolystictus","Cravus","Ctlaloci","Ctransversus")
rowcrot=c("Caquilus","Carmstrongi","Ccampbelli","Cintermedius","Cpolystictus","Cravus","Ctlaloci","Ctransversus")
colcrot
rowcrot
colnames(data) <- colcrot
colnames(data) <- colcrot
data 
str(data)
data2=as.matrix(data)
heatmap(data2)
install.packages("pheatmap")
library(pheatmap)
pheatmap(data)
heatmapdata=pheatmap(data, cluster_rows=FALSE)
heatmapdata=pheatmap(data, cluster_cols=FALSE)
heatmapdata=pheatmap(data, cluster_cols=FALSE)
heatmapdata=pheatmap(data, cluster_rows=FALSE,display_numbers = TRUE)
heatmapdata=pheatmap(data, cluster_rows=FALSE,display_numbers = TRUE, number_color = "black")
heatmapdata=pheatmap(data, cluster_rows=FALSE,display_numbers = TRUE, number_color = "black", angle_col = 45,angle_row=45)
heatmapdata=pheatmap(data, cluster_rows=FALSE,display_numbers = TRUE, number_color = "black", angle_col = 45, fontsize_number = 8, cluster_cols=FALSE, color = hcl.colors(50, "BluYl")) 
save_pheatmap_pdf <- function(heatmapdata, filename, width=7, height=7) {
save_pheatmap_pdf(heatmapdata, "heatmapunfilling.pdf")
RStudioGD 
        2 
setwd("C:/Users/Alumno/Desktop")
save_pheatmap_pdf <- function(heatmapdata, filename, width=7, height=7) {
setwd("C:/Users/Alumno/Desktop")
save_pheatmap_pdf <- function(heatmapdata, filename, width=7, height=7) {
save_pheatmap_pdf(heatmapdata, "heatmapunfilling.pdf")
RStudioGD 
        2 



============================================================ VARCROT ==============================================================

library(ggplot2)
library(ggstatsplot)
library(readr)
varcrot2_2_ <- read_csv("C:/Users/Alumno/Desktop/varcrot2 (2).csv")
View(varcrot2_2_)
ggbetweenstats(
+     data = varcrot2_2_,
+     x = Sitio,
+     y = Altitud,
+     type = "parametric", # ANOVA or Kruskal-Wallis
+     var.equal = TRUE, # ANOVA or Welch ANOVA
+     plot.type = "box",
+     pairwise.comparisons = TRUE,
+     pairwise.display = "significant",
+     centrality.plotting = TRUE,
+     bf.message = TRUE



# LEO
