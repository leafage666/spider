 - ����scrapy��ȡ��������(http://www.jobbole.com/)�µ��������ݣ����Ҵ��뱾�ص�mysql���ݿ��С�

 - ����spider���ݿ⣬��������ؽṹ��
```
SET FOREIGN_KEY_CHECKS=0;

-- ----------------------------
-- Table structure for jobboleblog
-- ----------------------------
DROP TABLE IF EXISTS `jobboleblog`;
CREATE TABLE `jobboleblog` (
  `title` varchar(200) NOT NULL,
  `create_date` datetime DEFAULT NULL ON UPDATE CURRENT_TIMESTAMP,
  `url` varchar(300) NOT NULL,
  `url_object_id` varchar(50) NOT NULL,
  `front_image_url` varchar(300) DEFAULT NULL,
  `front_image_path` varchar(300) CHARACTER SET utf8mb4 DEFAULT NULL,
  `comment_nums` int(11) NOT NULL DEFAULT '0',
  `fav_nums` int(11) NOT NULL DEFAULT '0',
  `praise_nums` int(11) NOT NULL DEFAULT '0',
  `tags` varchar(100) DEFAULT NULL,
  `content` longtext CHARACTER SET utf8mb4 NOT NULL,
  PRIMARY KEY (`url_object_id`)
) ENGINE=InnoDB DEFAULT CHARSET=utf8;
SET FOREIGN_KEY_CHECKS=1;
```



 - �޸�settings�µ�������ݿ����ã���������main����������ȡ���档