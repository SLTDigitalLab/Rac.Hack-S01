# Dataset 1: MQTT Protocol Data

## Dataset Description

The provided dataset contains MQTT protocol data collected from 8 sensors. MQTT (Message Queuing Telemetry Transport) is a lightweight messaging protocol commonly used in IoT (Internet of Things) applications. The dataset includes various features that describe the characteristics of the MQTT messages.

## Columns

The dataset consists of the following columns:

- `tcp.flags`: Flags associated with the TCP (Transmission Control Protocol) packets.
- `tcp.time_delta`: Time duration between consecutive TCP packets.
- `tcp.len`: Length of TCP packets.
- `mqtt.conack.flags`: Flags associated with the MQTT Connect Acknowledge packets.
- `mqtt.conack.flags.reserved`: Reserved flag within MQTT Connect Acknowledge packets.
- `mqtt.conack.flags.sp`: Session present flag within MQTT Connect Acknowledge packets.
- `mqtt.conack.val`: Value associated with MQTT Connect Acknowledge packets.
- `mqtt.conflag.cleansess`: Clean session flag within MQTT Connect packets.
- `mqtt.conflag.passwd`: Password flag within MQTT Connect packets.
- `mqtt.conflag.qos`: Quality of Service (QoS) flag within MQTT Connect packets.
- `mqtt.conflag.reserved`: Reserved flag within MQTT Connect packets.
- `mqtt.conflag.retain`: Retain flag within MQTT Connect packets.
- `mqtt.conflag.uname`: Username flag within MQTT Connect packets.
- `mqtt.conflag.willflag`: Will flag within MQTT Connect packets.
- `mqtt.conflags`: Flags associated with MQTT Connect packets.
- `mqtt.dupflag`: Duplicate flag within MQTT packets.
- `mqtt.hdrflags`: Header flags within MQTT packets.
- `mqtt.kalive`: Keep-alive value within MQTT packets.
- `mqtt.len`: Length of MQTT packets.
- `mqtt.msg`: MQTT message content.
- `mqtt.msgid`: Message ID associated with MQTT packets.
- `mqtt.msgtype`: Message type within MQTT packets.
- `mqtt.proto_len`: Length of the MQTT protocol.
- `mqtt.protoname`: Name of the MQTT protocol.
- `mqtt.qos`: Quality of Service (QoS) level within MQTT packets.
- `mqtt.retain`: Retain flag within MQTT packets.
- `mqtt.sub.qos`: Quality of Service (QoS) level for subscriptions within MQTT packets.
- `mqtt.suback.qos`: Quality of Service (QoS) level for subscription acknowledgement within MQTT packets.
- `mqtt.ver`: Version of the MQTT protocol.
- `mqtt.willmsg`: Will message within MQTT packets.
- `mqtt.willmsg_len`: Length of the will message within MQTT packets.
- `mqtt.willtopic`: Will topic within MQTT packets.
- `mqtt.willtopic_len`: Length of the will topic within MQTT packets.
- `target`: The target variable to be predicted. It can be classified as `legitimate`, `dos`, `slowite`, `bruteforce`, `malformed`, or `flood`.

## Task

The task at hand is to train a model that can accurately predict the target variable. The target variable represents the classification of MQTT traffic into different types: `legitimate`, `dos` (Denial of Service), `slowite` (Slow Read attack), `bruteforce`, `malformed`, and `flood`.

To accomplish this task, you need to apply machine learning techniques using Raccoon-AI engine to analyze the provided dataset and develop a model that can effectively classify MQTT traffic based on the given features.

For more detailed information about the dataset and its features, you can refer to the provided link: <https://www.mdpi.com/1424-8220/20/22/6578/htm>

**Note**: Please ensure that you have access to the Raccoon-AI engine and its documentation for more specific instructions and guidelines on how to utilize its functionalities to create the desired model.

- Documentation: <https://docs.raccoon-ai.io/>
- Raccoon-AI Engine: <https://engine.raccoon-ai.io/>
- Console: <https://console.raccoon-ai.io/>

## Files

- **train-set.csv** - The training dataset that you will use to train your model.
- **test-set.csv** - The test dataset that you will need to make predictions on and submit for the evaluation.
- **sample_submission.csv** - A sample submission file in the correct format that you will need to follow when submitting your predictions for the evaluation. (Rename this file to `submission-<team_name>-<dataset_1>.csv` before submitting your predictions.)
