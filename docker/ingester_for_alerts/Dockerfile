FROM public.ecr.aws/lambda/python:3.11

COPY ingester_for_alerts.py ${LAMBDA_TASK_ROOT}
COPY requirements.txt .
COPY sf-class2-root.crt .

RUN pip install -r requirements.txt

CMD [ "ingester_for_alerts.lambda_handler" ]