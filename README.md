###### BLOG DE SALUD 
## LOGIN USUARIO: admin Y PASSWORD: 10076465
![login](https://user-images.githubusercontent.com/54158226/83209485-81fea580-a126-11ea-93c7-752e42422efe.png)
## PANEL
![panel](https://user-images.githubusercontent.com/54158226/83209914-79f33580-a127-11ea-9eb2-84cbd9a0460f.png)
## ELIMINAR
![eliminar](https://user-images.githubusercontent.com/54158226/83209939-87102480-a127-11ea-8ecf-3d43d93e475a.PNG)
## EDITAR
![editar](https://user-images.githubusercontent.com/54158226/83209963-998a5e00-a127-11ea-80de-504988d6ffbb.PNG)
## EDITANDO
![editando](https://user-images.githubusercontent.com/54158226/83209975-a1e29900-a127-11ea-82ef-1030f0bd566e.PNG)
## NUEVO/EDITAR ENTRADA
![nuevo](https://user-images.githubusercontent.com/54158226/83209986-a7d87a00-a127-11ea-8dbb-511f2d774e04.PNG)
# BASE DE DATOS
/*
Navicat MySQL Data Transfer
Source Server         : LOCAL
Source Server Version : 100316
Source Host           : 127.0.0.1:3306
Source Database       : practica4
Target Server Type    : MYSQL
Target Server Version : 100316
File Encoding         : 65001
Date: 2020-05-28 21:16:32
*/

SET FOREIGN_KEY_CHECKS=0;

-- ----------------------------
-- Table structure for salud
-- ----------------------------
DROP TABLE IF EXISTS `salud`;
CREATE TABLE `salud` (
  `id` int(11) NOT NULL AUTO_INCREMENT,
  `fecha` date DEFAULT NULL,
  `titulo` varchar(255) COLLATE utf8_unicode_ci DEFAULT NULL,
  `contenido` varchar(255) COLLATE utf8_unicode_ci DEFAULT NULL,
  PRIMARY KEY (`id`)
) ENGINE=InnoDB AUTO_INCREMENT=5 DEFAULT CHARSET=utf8 COLLATE=utf8_unicode_ci;

-- ----------------------------
-- Records of salud
-- ----------------------------
INSERT INTO `salud` VALUES ('2', '2020-05-06', 'COVID-19 SE EXPANDE EN BOLIVIA', 'El COVID-19 dio con sus primeros infectados en la ciudad de oruro, lo cual dio paso a una cuarentena en el pais para su expansion a nivel nacional, esto para precaver su contagio');
INSERT INTO `salud` VALUES ('4', '2020-05-10', 'COMO ESTAR BIEN DE SALUD', '        Segun medicos de Bolivia dicen que tener una buena alimentacion,hacer deporte sano son la mejor medicina para que tu cuerpo este estable y fuerte, para asi en un futuro no tengas dificultades en tu funcionamiento de tu metabolismo.        ');

-- ----------------------------
-- Table structure for usuarios
-- ----------------------------
DROP TABLE IF EXISTS `usuarios`;
CREATE TABLE `usuarios` (
  `usuario` varchar(255) COLLATE utf8_unicode_ci NOT NULL,
  `password` varchar(255) COLLATE utf8_unicode_ci DEFAULT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8 COLLATE=utf8_unicode_ci;

-- ----------------------------
-- Records of usuarios
-- ----------------------------
INSERT INTO `usuarios` VALUES ('admin', '10076465');
SET FOREIGN_KEY_CHECKS=1;




