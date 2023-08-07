FROM pytorch/pytorch:1.2-cuda10.0-cudnn7-devel
WORKDIR /model
COPY ./requirements.txt /model/requirements.txt
RUN pip install --no-cache-dir --upgrade pip && \
    pip install -r requirements.txt
COPY . .
ENTRYPOINT ["python", "model.py"]