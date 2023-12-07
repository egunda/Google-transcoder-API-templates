# transcoder-API-templates
These are transcoder API templates to build automation
please refer my blog (https://medium.com/@kabani.nazir/automate-your-vod-transcoding-at-scale-with-gcp-part-1-87503fdd3a9f) for more details

Please note that due to formatting issue, the -- is shown as a single long hyphen and the double quotes character is also changed. Please correct it while running gcloud command.
Also, note that location should be asia-south1 instead of asia-south-1

    gcloud transcoder jobs create \

    -- input-uri=”gs://transcoding-automation-source/file-name-with-extension” \

    — location=asia-south1 \

    — output-uri=”gs://transcoding-automation-output/filename-without-extension/” \

    — template-id=”hd-h264-hls-dash”
