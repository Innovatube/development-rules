# Database Schema Design Guidelines

## Column name

All column names should be snake case. e.g. `user_name`, `id`, `content`.
Never use abbreviation form because it's make hard to understand for others.
Column names should be descriptive and represent "what is the contents, and format".
If the content of column is URL, use "_url" postfix.

## Primary Key

Each table's primary key name should be `id`
And when you need to create relation, related name should be (table name)_id. ( e.g. `user_id`, `article_id` )

## Datetime fields

Columns which stores date and time, it should be named as `XXX_at`. Such as `created_at`, `registered_at`.

And use TIMESTAMP instead of DATETIME format in MySQL. Because DATETIME format cannot store timezone info. TIMESTAMP format is based on UTC.

## Enum
Never use ENUM. Because it's not extendable. Use string(varchar) and handle the contents in the code.

## Blobs
Never store binary data (Images, and so on ) in the table. Use Cloud Strage and store URLs only in the table.

## Never use _1, _2 like number postfix.
If you need to store "maximum 3 same kind of data in one table", you need to normalize, create another table to store these data to prepare the maximum size becomes 4 or larger.
