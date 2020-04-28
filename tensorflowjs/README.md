tensorflowjs on docker
---

I wanna use tensorflowjs or tensorflowjs_converter.

## Usage

 ```bash
$ docker run -v $PWD:/app -w /app amanoese/tensorflowjs \
  tensorflowjs_converter \
    --input_format=tf_saved_model \
    --output_format=tfjs_graph_model \
    --signature_name=serving_default \
    --saved_model_tags=serve \
    /mobilenet/saved_model \
    /mobilenet/web_model
 ```

 more option is [here](https://github.com/tensorflow/tfjs/tree/master/tfjs-converter).

