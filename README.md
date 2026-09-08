# devops_netology

1. git begin

2. Файл .gitignore в каталоге terraform заставляет Git игнорировать:

.terraform/ — каталог с точным именем .terraform и всё его содержимое;
*.tfstate — любые файлы, имя которых заканчивается на .tfstate;
*.tfstate.* — любые файлы, в имени которых есть .tfstate., а после неё — что угодно (например, terraform.tfstate.backup);
crash.log — файл с точным именем crash.log;
crash.*.log — файлы, имя которых начинается с crash., затем — любые символы, затем заканчивается на .log;
*.tfvars и *.tfvars.json — любые файлы, заканчивающиеся на .tfvars или .tfvars.json;
override.tf и override.tf.json — файлы с точными именами override.tf и override.tf.json;
*_override.tf и *_override.tf.json — любые файлы, имя которых заканчивается на _override.tf или _override.tf.json (то есть с произвольным префиксом перед _override);
.terraform.tfstate.lock.info, .terraformrc, terraform.rc — файлы с этими точными именами.

Символ * в каждом правиле — это «любая последовательность символов», как и указал ревьюер на примере *IGNORE*.