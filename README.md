# API-Quickstart
Create a transcription job from an S3 link

mutation simpleTranscriptionJob{
    launchSingleEngineJob(input: {
      engineId: "c0e55cde-340b-44d7-bb42-2e0d65e98255"
      #targetId: 123456789
      uploadUrl: "<uri>"
      fields: [
        { fieldName:"keywords", fieldValue:"" }
      ]
    }) {
      id
  }}
