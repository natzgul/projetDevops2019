# On pull l'image python taggé en version 3.7 depuis le repository Docker
FROM python:3.7

# On copie le script de génération de la donnée vers les conteneurs
ADD ./units/unit1/script.py /home/scripts/

# Copy du fichier qui va remplacer le cron
ADD ./units/unit1/initialize.py /home/scripts/

# On copie le fichier de conf de l'unité
ADD ./units/unit1/conf.json /home/config/

CMD [ "python", "/home/scripts/initialize.py" ]