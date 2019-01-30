FROM python:2
ADD api.py requirements.txt /
RUN pip install -r ./requirements.txt
CMD [ "./api.py" ]
EXPOSE 5000
HEALTHCHECK CMD curl --fail http://localhost:5000/ || exit 1
