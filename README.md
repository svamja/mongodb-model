# MongodbModel

A thin Model around MongoDB collections with easy bulk, pagination and lookup operations

### Installation


    npm install nodejs-mongodb-model

This will also install 'mongodb' as dependency.

### Basic Usage

    const MongodbModel = require('nodejs-mongodb-model');
    
    async function main() {
      Photos = await MongodbModel.model('photos');
      await Photos.insertOne({ name: 'flower.jpg' });
    }
    
    main();

